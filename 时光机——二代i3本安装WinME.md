实际上，即使是现在的KabyLake，安装9X也是可以的。本人刚才在自己的老本子上安装了Win ME,运行正常，但别指望能用，硬盘控制器和USB识别不了，光驱用不了，只是个能点亮的系统。以下是安装方法：
1.保证能在DOS下访问硬盘分区，也就是至少有一个分区是FAT32
2.把硬盘模式设为AHCI（你没看错，就是AHCI，IDE进不去系统！！）
3.进PE，把Win ME的安装文件复制到硬盘——DOS下不能识别光驱
4.进DOS，安装系统。文件复制完成后，编辑system.ini，限制内存。Win ME需要限制为1994M及以下
5.检测硬件过程会蓝屏一次，重启就好
整个过程可以在10-12分钟内完成
***
限制内存的方法：在system.ini的386Enh下加上MaxPhysPage=，后面接上内存页块数（16进制）。每个页块是4KB。比如要把内存限制为1335MB，计算方法：1335MB=1367040KB=341760页，341760转成16进制是53700，那么就是MaxPhysPage=53700
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4924651093/94de4f35349b033b1f49abb11cce36d3d739bd89.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4924651093/2b946b328744ebf820843354d0f9d72a6259a7dd.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4924651093/6d0187ff9925bc31d59c56f357df8db1c9137089.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4924651093/89e3183f6709c93ddd33599c963df8dcd3005489.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4924651093/f32afb83d158ccbff449e25110d8bc3eb33541dd.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4924651093/9d3036db81cb39db7f35303dd9160924a91830dd.jpg)
配置
i3 2310m 8G 500G GT520M
硬盘没有超过514085M，WinMe的FDISK可以正确识别容量，但不能安装在128G后面，否则只能用兼容模式访问。光驱不能用。用32位保护模式会提示krnl386.exe不能加载
装Win95的话，需要把K6-2 CPU不定解压出来放在安装文件目录下再装，或者先关了VT，打完补丁再开
装NT4的话，要用我的SP6集成版，同时先把C盘格式化成NTFS并调整到8G以下。装完系统后换上XP的引导文件，再调回原来的大小。不过软关机没办法，因为M$只提供了标准PC和多处理器PC两个HAL的软关机支持，而这2个HAL都跟这个本子不兼容
