一楼只能上图了
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4971421332/70ba421e95cad1c8bec63887763e6709c83d5102.jpg)
下面就开始了
1.把Vista SP0镜像解压到某个目录
2.打开win7 sp1和vista sp0的boot\和efi\microsoft\boot\两个目录，对照其下的文件（不包括子目录），vista没有的从win7盘里复制过来；vista有而win7没有的就删掉，反正把文件结构弄成一样的。（这一步纯粹是装13[开心]）最后弄出来就是这样子
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4971421332/e3381bd88d1001e9e023d2afb10e7bec55e7976d.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4971421332/fa55aa10728b47109ac93d6ccacec3fdfe0323a5.jpg)
***
3.从上面提到的两个目录中复制etfsboot.com和efisys.bin到一新目录，跟oscdimg放一起。（对照1楼的命令行，看出来了么）
4.admin打开cmd，按照命令行修改相关参数，生成iso。注意只改卷标、日期、源文件、目标iso等不重要的参数就行了，前面跟udfver102和双轨引导相关的那些关键参数千万不能动
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4971421332/7a075d86e950352a7f56e7a85a43fbf2b3118b55.jpg)
***
生成iso的过程
最后生成的D:\9600Ent.iso就可以用来安装了
提示按任意键从CD或DVD启动
然后进入安装界面，注意壁纸和标题栏色调与sp1/2不同
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4971421332/90566bf531adcbefbae5b3a6a5af2edda1cc9fb7.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4971421332/990db02b6059252d7eb2d0a43d9b033b59b5b9db.jpg)
***
看到了么？前两个分区没显示（装好了重新进安装程序截图的[吐舌]
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4971421332/d8d6150f0cf3d7cae23af3d6fb1fbe096963a9bc.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4971421332/0cfc09071d950a7b7b91826403d162d9f0d3c9e4.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4971421332/01c0f00b304e251f9a8f2858ae86c9177e3e530f.jpg)
看到了么？winload.efi和6.0.6000
本帖结束
@happymax1212 可以试试实体机和u盘安装
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4971421332/b7f7f68ea0ec08fad752dd0750ee3d6d54fbda32.jpg)
oscdimg 2.56（32位）和win7的双轨引导文件我打包上传了（引导文件vista sp0没有）
链接：![](http://pan.baidu.com/s/1geLKCvD 密码：px78
@happymax1212 
efi装的vista不是很完美
1.bootmgr没有内存诊断
2.F8/F10菜单是英文
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4971421332/bd0ec850f3deb48f5c8d877ff91f3a292ff578a4.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4971421332/8be72e550923dd54b62181c9d809b3de9d824832.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4971421332/8eeffa17fdfaaf513d07a71e855494eef21f7aa4.jpg)
