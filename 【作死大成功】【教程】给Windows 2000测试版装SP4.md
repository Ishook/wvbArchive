下面以2183为例。
0.备份好`%systemroot%/system32/kernel32.exe`。
1.在系统中安装我提供的MainPart里的`Win2KSp4_en.msi`。如果有如下两图这样的错误（哪怕各不止一个）都可以无视。
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5256100160/745c39de8db1cb1314aa9bead754564e90584b79.jpg) 
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5256100160/3b006dd062d9f2d3b4308216a3ec8a136227cc18.jpg)

***
2.重启，打开一个PE。将我提供的Supplementary里的所有文件和文件夹直接覆盖式拖进`%systemroot%\system32\`，并用备份的`kernel32.dll`覆盖新装的`kernel32.dll`。
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5256100160/4c23f62297dda14485a5cd4bb8b7d0a20ef48694.jpg)

***
3.PE一般有提供引导修复工具，用它修复一下引导。
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5256100160/e9835e13b31bb0513ea812d13c7adab448ede0b5.jpg) 
修完以后要打开`boot.ini`确认一下修复得没问题。Windows 2000的安装目录一般是`*:\WINNT\`，但是有的引导修复工具会误写作`*:\WINDOWS\`。
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5256100160/5ab8360ed9f9d72a6acdb0e4de2a2834369bbb97.jpg)

***
4.再重启。正常启动Windows 2000即可。如果出现如下的错误提示不需害怕，只要按Ctrl+Alt+Delete进入安全界面，打开任务管理器再用它开`explorer`即可。当然也很可能根本不会出现这个错误提示。
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5256100160/191a5a6c55fbb2fbb3fdfbeb454a20a44423dc6f.jpg)

***
简单吧。
完[滑稽]——开个玩笑。
MainPart和Supplementary的下载：https://pan.baidu.com/s/1geNqgIB

***
@cghvbnv22 @兰兰和随随 @xkai @微軟藍澤光 @NZJ17001
@redapple0204 2167弄出来这个样子，要不是水印和炸弹还在我都不敢认了[狂汗]
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5256100160/0cfc09071d950a7bc99edd3d00d162d9f0d3c992.jpg)
***
测试了一下，部分地方达不到和SP4完全一致的效果，不过现在可以直接把SP4的exe拿来安装了。也就是说如果要更逼真可以用常规办法再装一遍SP4。
