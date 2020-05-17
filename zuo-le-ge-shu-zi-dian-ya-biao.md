# 做了个数字电压表

学校的古老指针电压表太辣鸡，我一气之下做了个数字电压表。算是对单片机资源（ADC）的充分利用吧。 第一位是数字的个位，后面是小数部分，如图读数是4.455V，比指针电压表不知道精到哪里去了\[滑稽\]只是由于数码管问题小数点不能显示，太可惜了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5394048838/c2d2a8fd1e178a8206e0d8fbfd03738dab77e887.jpg)

演示视频还在等审核。

诶，就加精了？那我赠送一下源代码吧

```c
#include "STC15.h"
#include "typedefine.h"

uint16 code Vbg_ROM _at_ 0x33f7;

sbit LP0 = P3 ^ 4;
sbit LP1 = P3 ^ 7;
sbit LP2 = P2 ^ 0;
sbit LP3 = P1 ^ 2;
sbit PinA = P3 ^ 5;
sbit PinB = P3 ^ 6;
sbit PinC = P2 ^ 1;
sbit PinD = P1 ^ 3;
sbit PinE = P1 ^ 7;
sbit PinF = P1 ^ 4;
sbit PinG = P1 ^ 6;
sbit PinH = P1 ^ 5;
unsigned char code NumVal[10] = {
0xEE,0x24,0xBA,0xB6,0x74,0xD6,0xDE,0xA4,0xFE,0xF6 };
uint8 counter = 0;
uint16 BGcache[3] = { 0 };
uint16 Acache[3] = { 0 };
unsigned int _100us = 9999;

int value = 0;

unsigned char DisplayTemp[4] = { 0xEE,0xEE,0xEE,0xEE };
unsigned char DisPosition = 0;
unsigned char DisPos2 = 0;

extern void display(void);

void ADCInterrupt(void) interrupt 5
{
    ADC_CONTR &= 0xEF;

    switch (counter)
    {
    case 0x10: {BGcache[0] = ADC_RES; BGcache[0] <<= 8; BGcache[0] += ADC_RESL; break; }
    case 0x20: {BGcache[1] = ADC_RES; BGcache[1] <<= 8; BGcache[1] += ADC_RESL; break; }
    case 0x30: {BGcache[2] = ADC_RES; BGcache[2] <<= 8; BGcache[2] += ADC_RESL; break; }
    case 0x40: {Acache[0] = ADC_RES; Acache[0] <<= 8; Acache[0] += ADC_RESL; break; }
    case 0x50: {Acache[1] = ADC_RES; Acache[1] <<= 8; Acache[1] += ADC_RESL; break; }
    case 0x60: {Acache[2] = ADC_RES; Acache[2] <<= 8; Acache[2] += ADC_RESL; break; }
    default: {break; }
    }
}

void timer2() interrupt 12
{
    uint32 temp1, temp2, FinalData;
    uint32 temp3;

    _100us--;
    if (_100us == 0)
    {
        _100us = 99;
        counter++;
        ADC_CONTR = 0x88;
        if (counter == 0x40)
            P1ASF = 0x01;

        if (counter > 0x60)
        {
            counter = 1;

            temp1 = (BGcache[0] + BGcache[1] + BGcache[2]) / 3;
            temp2 = (Acache[0] + Acache[1] + Acache[2]) / 3;
            temp3 = Vbg_ROM;
            FinalData = (temp2 * temp3) / temp1;
            FinalData = FinalData * 26 / 25;//The calvulated value is smaller than actual.

            DisplayTemp[0] = NumVal[FinalData / 1000 % 10] | 0x01;
            DisplayTemp[1] = NumVal[FinalData / 100 % 10];
            DisplayTemp[2] = NumVal[FinalData / 10 % 10];
            DisplayTemp[3] = NumVal[FinalData % 10];

            BGcache[0] = 0;
            BGcache[1] = 0;
            BGcache[2] = 0;
            Acache[0] = 0;
            Acache[1] = 0;
            Acache[2] = 0;

            P1ASF = 0x00;
        }
    }

    display();
}

void display(void)
{
    unsigned char temp = DisplayTemp[DisPosition >> 3] & (0x80 >> (0x07 - (DisPosition & 0x07)));

    PinA = 0;
    PinB = 0;
    PinC = 0;
    PinD = 0;
    PinE = 0;
    PinF = 0;
    PinG = 0;
    PinH = 0;

    switch (DisPosition & 0x07)
    {
    case 7: {PinA = temp; PinH = 0; break; }
    case 6: {PinB = temp; PinA = 0; break; }
    case 5: {PinC = temp; PinB = 0; break; }
    case 4: {PinD = temp; PinC = 0; break; }
    case 3: {PinE = temp; PinD = 0; break; }
    case 2: {PinF = temp; PinE = 0; break; }
    case 1: {PinG = temp; PinF = 0; break; }
    case 0: {PinH = temp; PinG = 0; break; }
    default:break;
    }
    switch (DisPosition >> 3)
    {
    case 0: {LP0 = 0; LP3 = 1; break; };
    case 1: {LP1 = 0; LP0 = 1; break; };
    case 2: {LP2 = 0; LP1 = 1; break; };
    case 3: {LP3 = 0; LP2 = 1; break; };
    }

    DisPosition++;
    DisPosition &= 0x1F;

    return;
}

void main(void)
{
    P2M0 = 0x03;
    P2M1 = 0x04;
    P3M0 = 0xF0;
    P3M1 = 0x00;
    P1M0 = 0xFC;
    P1M1 = 0x03;

    AUXR |= 0x04;
    T2L = 0xA0;
    T2H = 0xF6;
    IE2 |= 0x04;
    AUXR |= 0x10;
    EA = 1;
    EADC = 1;
    P1ASF = 0x01;
    CLK_DIV |= 0x20;
    ADC_CONTR = 0xC0;

    while (1);
}
```

材料：IAP15W413AS一个、4位共阴数码管一个、10μF电容一个（可选）、面包板一个、导线若干。 制作方法： 1.把单片机插在面包板上，烧好程序，烧录时内部晶振频率设置为24MHz，勾上“在程序区的结束处添加重要测试参数”。 2.按照如图的脚位对应关系把4位数码管插上去。（图见楼下） 3.在P1.0脚引出一根线作为正极测量针，在GND引出一根线作为负极测量针。 4.（可选）在P1.0与GND之间加一个10μF电容。 说明：1.单片机不能用同系列的其他型号如STC15W408AS替换，因为涉及到ROM里“重要测试参数”的地址问题。除非你对程序作相应修改。（修改方法这里不给出） 2.如果要用共阳数码管，也需要对程序进行修改。 3.加电容是为了\(1\)电压表表针悬空的时候示数不乱跳；\(2\)在电压表离开被测电路后还能短暂保存示数。 演示视频见 [https://www.bilibili.com/video/av15791003/](https://www.bilibili.com/video/av15791003/)

