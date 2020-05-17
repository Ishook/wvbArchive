# 其实电脑被激活问题锁住也可以进去的

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/9d3036db81cb39dbbddc4d99da160924a91830d1.jpg) 基本思路：想办法打开IE，然后再想办法找一个能操作文件的地方，最后通过它设法开explorer。 Longhorn 3713下是这样的：（XP差不多） Win+U仍然可以打开Utilman。用它打开Narrator，发现有个Microsoft Web Site。（平时估计大家都觉得这个链接很废柴……然而还真这么有起作用的时候） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/36fd2c37acaf2edd04d25c26871001e93b0193d7.jpg)

点进去，IE出来了。（网页本身打不开不要紧） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/ef371e300a55b319c1da96ba49a98226cdfc17d6.jpg)

看到这个了没？这是关键之一。能开出记事本就很可能能开出Explorer了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/0b0f9cecab64034f5c3fd6c9a5c3793108551d07.jpg)

点开，然后点击“Save As……” ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/e4fb2cfafbedab6421545a0ffd36afc37b311ecb.jpg)

下面一步也比较关键，把文件格式从.txt换成所有格式。不然到时候找不着Explorer。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/141351d02f2eb9382a336d3ddf628535e7dd6f9c.jpg)

选好以后，定位到`%systemroot%\`，就可以找到Explorer。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/75dea15d1038534374d591ee9913b07ec88088d8.jpg)

然后右键-open（打开），\[滑稽\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/07e4de13c8fcc3ce34a7dffc9845d688d63f208b.jpg)

这时候就可以去打开一个激活软件进行马后炮的激活了。当然只要网络能用，当场上网下载一个使用也是可以的。不过注意，XP~Longhorn这样强行打开Explorer以后，不久系统会又把Explorer关闭，到时候就还得重复一遍来打开Explorer了。 再用Windows 7 6608演示一下。这个复杂一点，学会这个以后对NT6的这类界面就不用担心了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/8b1b11084b36acafa4a39f3376d98d1003e99cb7.jpg)

点击第一项。系统会自动打开IE。如果实在没有如图第一项，下面还有个Read our privacy online也可以开IE。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/e8279a1e4134970af89018e09fcad1c8a5865d17.jpg)

Page下有个Save As...，一样打开。（Vista~早期Win7可能要用左下角的Browse Folders手动展开界面） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/cb20d41d8701a18ba19a1980942f07082a38fe85.jpg)

然后坑爹的事情来了，你不能选择“所有格式”。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/4e007cd4ad6eddc4b84dbf3433dbb6fd50663348.jpg)

这种时候就要动动脑筋了。选择txt，然后随便乱存一个。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/f32afb83d158ccbfd687bff513d8bc3eb035413f.jpg)

存完以后，这个文件浏览窗口就关掉了，那存这个有什么用呢？继续往下看。

再次打开Save As...，还是选择txt，定位到你刚才保存txt的目录，然后就可以看到刚才的东西。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/65ebf2cbd1c8a78600d23ec16d09c93d72cf507e.jpg)

右键单击这个txt文件。右键-打开。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/d53eb6c9a786c917b5fb26f6c33d70cf39c7577e.jpg)

你应该能明白该怎么做了\[滑稽\]\[茶杯\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/913cc087c9177f3eaccc88c27acf3bc79d3d567e.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/e772ae167f3e670905f8313031c79f3dfadc557e.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5299807814/89e3183f6709c93dbd0a7a38953df8dcd300547e.jpg)

顺带一提，诸如6608这样的系统尚无什么激活办法，但是在Vista以来，这样强行打开的Explorer不会像XP一样被系统捣乱关闭。所以，调出资源管理器后，把IE什么的关掉，把激活那个窗口（激活的窗口仍然不可以关不然还是要注销）最小化，然后就假装你已经激活过，美滋滋地用吧\[滑稽\] \[OK\] 完。 XP的办法网上貌似有人找出了类似的办法，不过没我机智，他可没能打开Explorer\[滑稽\] 后面那个办法好像网上还没有

既然NZJ认为价值偏少,我再追加一些微小的补充:在中文版XP中,还有一种理论可行的办法。如果你正巧在之前把语言栏从任务栏分离了出来,那么系统锁机要求激活时语言栏应该还能显示。可以在语言栏上面开MSPY的自造词工具。它可以导入词库文件,然后查看文件时可以选择所有格式。这样,它也可以找到Explorer而启动资源管理器。

