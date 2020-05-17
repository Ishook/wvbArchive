从XP开始，格式化软盘的时候可以选择“创建MS-DOS启动盘（M）”，8.1还保留了这个功能，但10不见了。实际上，这个功能只是隐藏了，用访问键还能操作。只要把8.1的diskcopy.dll复制到10里，这个功能就恢复了，操作时按Alt+M，看到选项都变灰，就说明已经选中那个选项了。此时点开始，即可完成DOS启动盘的制作。这个启动盘是WinME启动盘的精简版。IBM原装USB软驱测试通过
目前需要恢复的是Win10的复制软盘功能
所以保留下来的DOS启动盘完整版应该这样做：
1.用系统自带功能格式化一张DOS启动盘
2.diskcopy.dll复制到软盘上，改名为ebd.cab
3.XPSP3 的deploy.cab里解压oformat.com复制到软盘上，改名为format.com
但这样做出来的还是缺少一些内容，比如fdisk和光驱驱动
这个启动盘可以刷bios，我刷过award的。把awdflash.exe和bios数据文件复制到软盘，再建立一个autoexec.bat，写上awdflash xxx.bin /sn /py /cd /cc /cp /r，用他启动电脑即可
截图演示：
我已经提取了2012R2的diskcopy.dll到2016
格式化软盘，按Alt+M，可以看到选项全灰了，这就相当于选中了创建MS-DOS启动盘，下面的空白处就是阉割掉的那个选项原来的位置；再按Alt+M，又能恢复原状。顺便提一下，NT6已经不能在格式化时启用压缩了，格式化硬盘也不行
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4890623370/43cf3cb4c9ea15ced8ed6e16bf003af33b87b2a0.jpg)
***
然后点Start，格式化过程比较慢，而Quick Format是被选中的，明显各种设置都没有起作用，实际的动作只是释放diskcopy.dll里的软盘镜像
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4890623370/bcf7f544d688d43fe30518ed741ed21b0ff43b72.jpg)
***
格式化后
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4890623370/50cc3442fbf2b2116b170d51c38065380dd78eee.jpg)
