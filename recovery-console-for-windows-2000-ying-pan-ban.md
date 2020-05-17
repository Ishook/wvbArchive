# Recovery Console for Windows 2000（硬盘版）

好久没折腾技术了\[吐舌\]今天奉上一个技术向新作品 玩过老系统的人应该对启动软盘的Recovery Console不陌生。当系统出问题的时候，它是一个维护利器。 可惜，这个东西只有从软盘或者光盘启动才能进入。这一次，我以官方Windows 2000软盘为材料，经过精心高汤料理（划掉）经过精心制作，终于使其具有了从硬盘启动的能力。我还编写了一个批处理脚本，可进行一键安装，使用极其方便。 效果镇楼 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5565871259/4c07b0cb7bcb0a46cf68ea1c6763f6246a60af46.jpg)

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5565871259/730ee58aa61ea8d3517715219b0a304e241f58b7.jpg)

本次制作的Recovery Console for Windows 2000仅适用于Windows 2000。

不过，虽然它基于Profession的软盘制作，它可以适用于各个SKU。 共提供四个软盘文件包，其文件提取自四个不同Builid的Windows 2000的软盘。其中Build 2031那个已经确认有一些问题，不建议使用。其他三个均可以使用，它们三个之间Build不同完全不影响使用，完全通用，之所以提供三个只是因为我有系统收集癖。 下载地址： [https://pan.baidu.com/s/1c2O9Sje](https://pan.baidu.com/s/1c2O9Sje)

使用方法： 1.下载grldr和setup.bat两个文件，再任取一个软盘文件包下载即可。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5565871259/141351d02f2eb938e11818d7d9628535e4dd6f97.jpg)

2.解压软盘文件包，得到files文件夹。请注意保持files文件夹与另外两个文件处于同一目录。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5565871259/f7b124a88226cffce97add97b5014a90f703eabd.jpg)

3.直接拿到Windows 2000中，打开setup.bat安装即可。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5565871259/4a8f65097bf40ad17969a5c65b2c11dfa8ecce7f.jpg)

重启后即见到新增的启动项。这个启动项是新添加的，完全不会影响原有任何启动项正常使用。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5565871259/47fc4f391f30e924a984f11440086e061c95f7ec.jpg)

选择后者进入后，会有一段时间的黑屏，这时候是（Recovery Console的）系统正在启动，不需要担心。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5565871259/65ebf2cbd1c8a786661f262b6b09c93d71cf50d7.jpg)

然后是我们熟悉的界面了。这个时候不要手贱按Enter——为了进入Recovery Console，应该按R键。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5565871259/94de4f35349b033b107891ff19ce36d3d439bd1c.jpg) 接下来到了这里，经过测试，按C和按R两种修复方式都可用，都可以试试。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5565871259/303b5cc69f3df8dc6622e3b4c111728b461028e9.jpg) 按R就会来到Recovery Console了\[haha\]\[滑稽\]\[胜利\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5565871259/89e3183f6709c93dc3ed62d2933df8dcd00054e9.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5565871259/c5c182dce71190ef09e4fefac21b9d16fcfa60e9.jpg)

\*附赠的技术信息 1.本恢复环境的工作原理： 由NTLDR引导一个我自定义的BOOTSECT.DOS文件，这个自定义的BOOTSECT.DOS文件会引导同目录下的grldr，grldr会引导SETUPLDR.BIN，SETUPLDR.BIN最终引导恢复环境。 2.卸载方法： 这个东西不会写入注册表，惟一对系统设置的更改就是在boot.ini写入了一条启动项。所以卸载时只要把复制到电脑上的文件手动删除，并手动编辑boot.ini删掉启动项即可，这不会很麻烦。

如果想要知道我是怎么做出这个东西的，可以参考 ![](http://tieba.baidu.com/p)

写在最后：WindowsNT吧已经光复！欢迎各位吧友有空的时候到WindowsNT吧坐一坐。本作品的制作过程就初载于WindowsNT吧。 ![](http://tieba.baidu.com/f?ie=utf-8&kw=windowsnt)

