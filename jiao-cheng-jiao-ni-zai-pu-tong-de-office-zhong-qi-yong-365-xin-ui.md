# 【教程】教你在普通的office中启用365新ui

不知从什么时候开始，ｏｆｆｉｃｅ２０１６ 零售版不在推送新功能了，原来推的那些功能比如黑色主题、ppt的设计构想之类的都扔给了３６５，现在２０１９发布在即，由于是c2r自动更新的，所以很多吧友已经用上，并换上了不会过期的正式版号码，但２０１９也只具备原来推送的一部分功能，推送过的并不是全部都有。比如黑色主题、ｅｘｃｅｌ的新函数是有的，ppt的设计构想依然没有。由于２０１６ ２０１９ ３６５的安装文件、版本号都是一模一样的，所以猜想是不是类似ｗｉｎ１０那样，通过证书和ｋｅｙ区分版本。反复卸了装，n次折腾后，终于发现，原来这就是m$的阴谋。。。 下面就是具体方法： 首先，你要确保能正常使用ｋｍｓ集火ｏｆｆｉｃｅ，然后准备好ｏｔｐ软件和相关的ｋｅｙ（稍后放出）。 把原来的ｏｆｆｉｃｅ全卸了，安装２０１６ｍｏｎｄｏ这个版本。注意这是关键！只有这个版本配合３６５的证书才能启用新ｕｉ，否则只是图标和功能有更新，开始界面和标题栏还是旧的。。。当然直接换证书和ｋｅｙ也一样，但ｍｏｎｄｏ的优势在于，直接整合了ｐｒｏｊｅｃｔ和ｖｉｓｉｏ这两个从来不在ｏｆｆｉｃｅ套装里捆绑的软件，而且他俩授权贼贵，ｐｒｏｊｅｃｔ是１９０每月，ｖｉｓｉｏ是９５每月，已经赶上甚至超过了３６５ｐｒｏｐｌｕｓ的价格！ 装完后不要启动ｏｆｆｉｃｅ，直接清除原有的ｋｅｙ和证书（要先清除ｋｅｙ），然后安装２０１６ｍｏｎｄｏ ｖｌ和ｏ３６５ｐｒｏｐｌｕｓ的证书和ｋｅｙ。用ｏｔｐ安装不在列表前几位的证书（就是那些有复选框的证书）时是不会自动安装ｋｅｙ的，这时就需要手动安装ｋｅｙ了。当然感兴趣的话你也可把ｏｆｆｉｃｅ，ｐｒｏｊｅｃｔ，ｖｉｓｉｏ的２０１６＼２０１９零售＼批量版，ｏ３６５其他版本的杂七杂八的证书和ｋｅｙ都装上（我给的文件里都有，随你了，但２０１６ｍｏｎｄｏ和ｏ３６５ｐｒｏｐｌｕｓ的证书和ｋｅｙ是必须的），这样在ｏｆｆｉｃｅ程序里会同时显示几种授权，装高大上很有用。。。。这些操作都可以用ｏｔｐ完成 最后ｋｍｓ激活一下，让这些证书都生效，再运行ｏｆｆｉｃｅ就可以看到新ui了

效果： ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5846905913/592cdb3fb13533fa973e4119a5d3fd1f40345b76.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5846905913/94cbe095a4c27d1eeaf7e9f316d5ad6edcc4382d.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5846905913/8808a4cfc3fdfc03a0a8318fd93f8794a5c2262e.jpg)

注意：如果第一二次打开看不到新界面的话多打开几次 证书、key我就装了2016/2019的mondo、office、project、visio的（2019没有mondo）和o365四种版本的； 这样的好处在于，初始时装的是2016,他是支持win7/8的，这样可以一直接受更新。如果初始时装的是365又是win7/8，那么2020年以后就不能更新了，因为m$早已宣布365到时不再支持老系统，包括win10的ltsc、srv2016等。。。

office tool plus自备，激活推荐office 2013-2019 c2r install比较新的版本，注意不要再转换vl了，直接activate即可。我提供一个6.4.2的： 度盘/s/12DRX39ABAYX9jvCtXWv6hg 密码：uzq5

另外所需的key在这个txt里： 前面省略/s/1trZoWGe8tS0Sgjt7Y-2YQQ 密码：mr81

补一张我装的证书： ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5846905913/dc76b659ccbf6c818d72f3dfb13eb13532fa40b1.jpg)

经测试，正常卸载再重装，以及在线更新、重新kms都不影响授权信息，新ui新功能都有

再补充，win7, 8, 10都可以这么整。。。

office确实是通过证书来限制功能的。比如你装了2019，清除原有证书后换2016的证书和key，那么2019的新功能就没有了。2016换2019的证书和key，同样会开启新功能。比如插入3d模型、学习工具，一眼就看出来了 @vistawithsp2 @happymax1212 重要通知！想用2016mondo+365证书+365key的方式体验365ui的，必须使用快环或狗粮通道（建议快环），举例：同是1808，快环的10723已经是新ui，慢环的10730却是旧ui。可以用otp改更新通道 更新：从1902开始，所有office元件都有新ui了，1904开始有新图标，但只是word excel ppt outlook onenote五个，前提是mondo2016或365

