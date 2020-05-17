# 【中速】Windows 2000史——从Windows NT 4.0到Windows 2000

期末考试终于结束了，暑假赛高！！！！！！！！！！！！！ 我读过许多吧友整理的Windows各系统史，包括Vista史、XP史，但是一直没有看到过专门的2000史。这个暑假，让我们回到1997~1999的那段时光，回忆Windows 2000史吧！ 本帖特色：不使用来自TCB的图片，全部自己安装、截图。 特别感谢@cghvbnv22 提供系统下载和部分系统资料与界面评价。 通过神秘手段刷上VMware Tools的2183镇楼\[滑稽\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c722407e9e2f0708d4dd73b8e324b899ab01f2a0.jpg) 更帖原则： 先更WKS-PRO线，SRV线可能不会有。 部分太难装的不会装\[勉强\]。 只要有空，每天装3~10个Build。 Windows NT 4.0 Build 1386 阶段：post-RTM（？） 详细版本信息：？ 谜之Build。 这个版本非常古怪。光盘本身不能启动。从NT4打开升级提示缺少文件。使用winnt /b有如下错误： ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/79f5463eb80e7bec05c64859252eb9389a506b5b.jpg) 惟一能用的办法是DOS下winnt不加/b安装。那样这个Build安装前会先叫你创建启动软盘，然后才开始安装。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/bb06d5109313b07ef6b11fb006d7912396dd8c6b.jpg) 安装奇慢无比。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/89e3183f6709c93dfef9bb4f953df8dcd0005470.jpg) 这个安装程序真是差劲，连启动都没有弄好，我还是启动到了原来的DOS\[喷\] 目前正在琢磨怎么进入Windows。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/91b7ca4ad11373f03ac9dc27ae0f4bfbf9ed048d.jpg) \[狂汗\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/fefd0c62f6246b6002820dcce1f81a4c530fa2eb.jpg) 下面用一点非常规办法。 思路：用Windows NT 4.0光盘启动，安装，然后偷梁换柱，将1381的$WIN\_NT$.~LS文件夹替换成1386的。 结果…… ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/ebecf02ad40735fa7b76ee0194510fb30d2408fd.jpg) 雾草怎么是一样的问题\[惊哭\] 折腾了半天，终于把文件安上了。确实是NT5\[惊讶\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f32afb83d158ccbf3f36268213d8bc3eb33541f1.jpg)

接下来要解决的问题就是…… ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/36fd2c37acaf2edd826bda51871001e93b0193e1.jpg) 终于把1386安上了！！ 下面开始正式的评测。这一定是独家原创；正如NZJ所说，连TCB都没有收录！ Windows NT 4.0 Build 1386 阶段：post-RTM 编译日期：1996年11月16日 详细版本信息：谜，任何文件版本都是1381.1或1381.3，还有2006.\*，偏偏找不到1386.\*；在注册表找的的版本又是简单的“1386”，所以不能确定是不是1386.1。 下面是界面。 这是系统里少见的没有替换成“NT5”的地方。顺便赞一下那时候的开发者，刚刚做到比RTM Build大5的时候，已经把系统里其他绝大多数地方的“NT4”字样都换成了“NT5”，包括很多图片也都换了。不像后来开发Win8的时候，系统内大量残留“Windows 7”字样。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/2b946b328744ebf8c7f6ef87d3f9d72a6259a7fd.jpg) 看，连这个角落都换成NT5了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e4fb2cfafbedab6487f2b878fd36afc37b311eff.jpg) 这个Build都已经放上NT5的图片了，真负责。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/27fdae3c70cf3bc7d0ea3954db00baa1cf112a91.jpg) 水印是败笔……另外开始菜单的“Unicode Debug”挺显眼。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e772ae167f3e670985dab14731c79f3dfadc55a1.jpg) 文件资源管理器尚未改造成15xx的酷炫样式。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f9ccfc514fc2d56291182755ed1190ef77c66c6f.jpg) 成功装上显驱！来感受NT5专有的美丽。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f3e8e000a18b87d685935da70d0828381d30fdaf.jpg) 合照。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3c2dea1101e9390126497d8671ec54e737d19630.jpg) IE ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b7c2c8c279310a5531cd234cbd4543a980261096.jpg) 注册表有一个谜之键值。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d17bc7ed08fa513d9f789166376d55fbb0fbd9aa.jpg) 好了，不出意外的话，1386应该是全NT5最难装的。这个苦都吃过了，装其他的就显得容易多了。 Windows NT 5.0 Build 1515 阶段：pre-Beta 编译日期：1997年3月17日 详细版本信息：5.0.1515.1 这个Build神他喵没有winnt32.exe，然后还不可引导。那么喜闻乐见地……我又要从DOS启动安装了…… 普通的winnt /b安装。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4ab2951ebe096b634958bce806338744eaf8ac3f.jpg) 明明是RAMDisk，每次上winnt /b都会奇慢无比。。。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d8d6150f0cf3d7cac34cd3cef81fbe096963a9c2.jpg) 重启了。15xx这段似乎是默认打开了Debugging Mode。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/dfc99fddd100baa1fbbaac034d10b912cafc2eed.jpg) 终于要进入GUI了。这里已经完全换为“NT5”了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/68cc7831e924b8992231ad8064061d950b7bf66b.jpg) 看看，这多良心亲民\[滑稽\]\[大拇指\]真的比Whistler不知道高到哪里去了。 （看不懂可以自行使用翻译工具） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c7f5c68a87d6277f1f4fe28022381f30e824fc1b.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c6ec517bdab44aed54c26e5cb91c8701a38bfbf4.jpg) 忽然发现，NT4的非活动窗口标题栏的文字是灰色，NT5则是黑色，好像变难看了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/ab0c7d4d510fd9f9613088d12f2dd42a2934a45d.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/5fc48e25b899a901c902868e17950a7b0308f54d.jpg) 太晚了。明天继续。 来看看这个Active Desktop（\*我已经装过显驱） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f08aad8165380cd7b6600554ab44ad3458828106.jpg) 这是卖萌吗\[喷\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b0eb5d282df5e0fecf852eb8566034a85cdf72db.jpg) 改造过的explorer好评！尤其是那个“my computer”图标，超前地有扁平化风\[开心\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/dea568b20f2442a77c425b1cdb43ad4bd0130234.jpg) 所有图标上的名字（例如：文件的文件名，桌面的“My Computer”，explorer里的盘的卷标等）都做成了类似链接的样式，左键单击仅一下就可以进入。 下图我光标指中的就是：

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/6e87ecd5b31c87016f48125f2d7f9e2f0508ff87.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/8f0879168a82b901f473638a798da9773b12efa7.jpg) 即使指针在图标上图标上悬停了一会儿而没有点击，几秒钟之后系统也会自动将图标选中。如果你用过XP里那样的屏幕键盘，你就会知道那屏幕键盘里有一个“悬停自动当作点击”功能，和这个是差不多的。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e772ae167f3e6709bfb5e74631c79f3dfadc55c3.jpg) cghvbnv22：显示桌面位居任务栏右下角的设定在同时进行开发的Memphis build 1400～1415、以及后来的Windows 7，Windows 8以及Windows 10内均可以见到！\[真棒\]

好吧，其实我觉得这个不如后来NT6的那个好用。因为NT6的那个”显示桌面“按钮，看也不用看，只管把鼠标拉到屏幕最最右下角点击一下就行了。即使是经典主题，拉到最最右下角以后点两下也就行了。1515这里的按钮，把鼠标直接拉到最最右下角是点不到的，还得出来一点，也就是还要用眼睛看一下。那就麻烦了一点。 如图，鼠标在右下角，但是点不到那个按钮。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/95cdd1013af33a87fac6afa3cc5c10385143b5d1.jpg) 合照。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d17bc7ed08fa513dc288c467376d55fbb3fbd95b.jpg) 1515就到这里吧。 Windows NT 5.0 Build 1585 阶段：pre-Beta 编译日期：1997年3月17日 详细版本信息：5.0.1585.1 这个Build似乎不能从NT4升级\[吐\]幸亏这回可以从光盘启动了。 升级出现的错误。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b2ebd9086b63f6248446a4ba8d44ebf81b4ca362.jpg) 偷个懒啦。直接搬一下我另一个帖的图。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/07e4de13c8fcc3ceb134548a9845d688d63f208c.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f9e6affdc3cec3fd8fca3accdc88d43f8594278c.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/8808a4cfc3fdfc03e68c7e01de3f8794a6c2268c.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/833aa4fcfc039245a3417cb68d94a4c27f1e258c.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/90566bf531adcbef6dc6e3bfa6af2edda1cc9f8a.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4c0056accbef760957f9042624dda3cc7ed99e8a.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/7159acee76094b36b1608654a9cc7cd98f109d8a.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/973e1cca0a46f21f55cac2eafc246b600e33ae87.jpg) 这个Build一些图片会因为颜色位数不够直接不显示。。。此前的Build印象里都照顾老机比较好，没有出现过这种状况。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3b3f6d47f21fbe0987a05fad61600c338544ad87.jpg) 装上显驱以后 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/cde466e83901213f9c46d2655ee736d12e2e9503.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/411d5e00213fb80e5ea4fd6e3cd12f2eb8389403.jpg) 有时候刚登录的时候屏幕上会出现一个Windows徽标，可以拖动。不久后消失。作用不明。

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/768ebdb54aed2e733d7a19958d01a18b85d6faea.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/9a402dec2e738bd404b22d88ab8b87d6257ff9ea.jpg) 这个界面我个人感觉还不如1515，而且紫色图标是什么鬼\[汗\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/94f352fbe6cd7b89147fa53a052442a7d8330e69.jpg) 合照。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/678bf92e07082838a11442adb299a9014d08f160.jpg) 其他是cghvbnv22的发现： Setup更新好评，系统属性定型，显示桌面位居任务栏右下角的设定取消，同时Memphis build 1423也取消了显示桌面位居任务栏右下角的设定，Outlook Express首次出现。 1585到此为止。1592、1631是Server Only，暂时不装。 Windows NT 5.0 Build 1671 \(Workstation\) 阶段：pre-Beta 编译日期：1997年9月9日 详细版本信息：5.0.1671.1 不知道为什么，1671镜像的体积是1585的两倍。幸好这回可以从NT4升级了，不然我一口老血都要喷出来了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/43bb1ff1f736afc3e33ca4dcb919ebc4b6451248.jpg) 对了，安装界面的这个改进在1585就有了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/678bf92e07082838a3d344adb299a9014e08f1a7.jpg) 算了当我没说。这个Build还是不能从NT4升级的。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b6d00c610c3387443605a7c55b0fd9f9d52aa0b9.jpg) 我试着用安装光盘修复。 注意，15xx及以前好像不禁用ACPI还没事，但是最迟从16xx开始一定要处理一下了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/efa594dfb48f8c54b0b34f9630292df5e1fe7f18.jpg)

启动时已经不是Debugging Mode了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/43cf3cb4c9ea15cedf346ab0bc003af33887b2a3.jpg) 为了保住各种驱动等等，我不动注册表了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/191a5a6c55fbb2fb8601acab454a20a44723dc53.jpg)

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/cae7042662d0f7032de3616502fa513d2797c528.jpg) 修复流程顺利完成——只是没修好罢了…… ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/49d0cc19972bd40745a0274471899e510eb3091d.jpg) 我还是选择了从光盘全新安装。这样是没有问题的。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4ab2951ebe096b632586a8e906338744e9f8ace6.jpg) CD安装的话，就没有显驱了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3b7df9500fb30f2432ba1ebac295d143ac4b0358.jpg) 手动安装显驱好像不行。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d01b11c7a7efce1b88623573a551f3deb58f6537.jpg) 经过探索，发现这个Build几乎没有新功能。还这么难用，真是个渣。不用它了。 Windows NT 5.0 Build 1691 阶段：Beta1 编译日期：1997年10月24日 详细版本信息：5.0.1691.1 1691的镜像体积恢复了正常大小。 这个Build又没有winnt32\[弱\] 而且……又回到默认Debugging Mode了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/01c0f00b304e251fb5623641ad86c9177d3e53e3.jpg) 又玩我\[心碎\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/90e26e25ab18972b9cc7dd73eccd7b899c510afb.jpg) 吓得我用了DOS ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/1a5bc30e4bfbfbede72df4c672f0f736aec31f0c.jpg) 普通地安装 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/750e81cc7b899e51327ff7ad48a7d933ca950d8f.jpg)

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f9ccfc514fc2d56258661c54ed1190ef77c66c17.jpg) 它是从哪里看出AC Power的？！ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/8b1b11084b36acafe2b1594576d98d1000e99c28.jpg) 手动安装显驱继续蓝屏。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/750e81cc7b899e513550f4ad48a7d933ca950da6.jpg) 算了，这个Build反正也是乏善可陈……放弃它了。 cghvbnv22：这个版本的控制面板项内增加了Scanners and Camera，从而增加了对便携式设备的支持。而且字体也出现了变化。 下面…… Windows NT 5.0 Build 1729 阶段：Beta1 编译日期：1998年1月7日 （更严谨的叫法）版本字串：5.0.1729.1 有winnt32耶。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/cd45ac124954092301ec43c49858d109b1de49fc.jpg)

下面几步是一样的，界面没变。 重启。还是Debugging Mode。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/39c56d54b319ebc482c554238826cffc1f17163b.jpg) 终于有一个能正常升级的了（喜极而泣） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/967cb33e8794a4c277e2c59104f41bd5af6e39bf.jpg) 继续亲民233 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/95cdd1013af33a877c1d2da0cc5c10385243b509.jpg) 再次重启。诶，我的真彩色呢？（不好的预感） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/91b7ca4ad11373f0a7114325ae0f4bfbfaed0456.jpg) 啊！ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f2e5f412b07eca80fb27155d9b2397dda044835b.jpg) 看来还是SVGA驱动引起了问题。幸好我保留了一个尚未装入驱动的快照，不然得从头再来。（忽然发现我已经被快照救了无数次了） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/47fc4f391f30e924e92ab38b46086e061f95f7f7.jpg) 安装界面左下角怎么自己打开了一个cmd？玩会试试。（然而并没有成功玩出什么） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f7b124a88226cffc2b7b9108b3014a90f703ea28.jpg) 又一种不好的预感。不过至少可以看到右下角的登录显示的那个徽标样子变了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/11fbbef8d72a6059a72fcaa02234349b023bba46.jpg) Ouch！（again） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e9f52b096e061d955bd41d8271f40ad160d9caeb.jpg) 摸索了一下，发现desk.cpl那个报错是个炸弹，不能点；藏在下面那个是可以点的，然后会出现桌面环境。（不过任务栏呢= =b） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/7159acee76094b3609370e57a9cc7cd98f109ddc.jpg) 哎，还是从CD启动安装吧。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d9d1db305c6034a8e2c0bd3bc11349540823765b.jpg) 安装程序比起16xx又有变化。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b6d00c610c33874481912ac65b0fd9f9d62aa02d.jpg) 日历好生动【误 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/512bceed8a1363272913c7899b8fa0ec0afac787.jpg) 好了先进桌面再说。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/bb19cc65034f78f0e2069e4973310a55b2191c6b.jpg) 嘿，这里界面变了，找不到装显驱的地方了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/0253be32c895d143a42fe39979f082025baf0727.jpg) 设备管理器闪亮登场！（好评） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/06d76ef6905298222e603e79ddca7bcb0b46d42a.jpg) 妈呀这么多驱动缺失…… ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e4fb2cfafbedab6411ba4a7afd36afc37b311eb0.jpg) 界面尚属稚嫩。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/92ef69f51bd5ad6e2e4862508bcb39dbb4fd3cc8.jpg) 装了VBEMP还是16色……我可能需要重启。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/913cc087c9177f3ebf31fdb77acf3bc79e3d567c.jpg) 重启后没有蓝屏，但还是没有真彩色。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/91f4dda0cd11728ba7b68f98c2fcc3cec1fd2ce2.jpg) 显驱简直难弄到变态啊，一个下午也没装上 \(╯‵□′\)╯︵┴─┴我不弄1729了，还是上1743吧。 Windows NT 5.0 Build 1743 阶段：Beta1 编译日期：1998年2月5日 详细版本信息：5.0.1743.1 光看表面看不出什么很特异的地方。 能升级的侥幸心还是要抱的，万一成功了呢。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/2b9791256b600c33aadf8772104c510fdbf9a1df.jpg) 对了，我有一个发现。 这个界面按F8是没有什么用的。

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/7159acee76094b36f41f4357a9cc7cd98f109df4.jpg) 但是你按F5时，就能来到这里： ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/ebecf02ad40735fa25ce140394510fb30e240847.jpg) 它吓得我把1729重装了一遍，发现没有这个功能！这个功能就是1743的新功能。 因为感觉我手可能不够快，直接做成批处理好了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/2c75e70b19d8bc3e3a6c4170888ba61ea9d3451d.jpg) 然后灌进iso。启动安装，祝我好运！ 咦，照道理应该可以把那个VGA mode删掉不要单独立项了呀。怎么还留着。不管它了先进第一个再说。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/303b5cc69f3df8dc4e80c92bc711728b451028c4.jpg) 什么鬼呀这是！一启动就这样，我根本来不及反应。更坑的是这时候鼠标竟然动不了，Alt+Tab等键盘操作也不行。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/a529801090ef76c6c0c7ba919716fdfaae51676c.jpg) 哦哟，编BWDB的人真不知道是怎么回事。明明用普通启动才对，那样才不至于操作不了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/0a649102738da977d829c591ba51f8198718e378.jpg) 然后卡在这里（感到不解） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/1a5bc30e4bfbfbed60637bc572f0f736aec31f43.jpg) 看样子这系统不是在忙就是在死循环。lz先把它搁在那运转，吃过饭再回来看吧。 等了好久以后\[喷\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/70ba421e95cad1c8dafd459d753e6709c83d513f.jpg) 又等了很久……好像奇迹发生了\[惊哭\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/79e6d41ab051f8194ecfa5f0d0b44aed2c73e79c.jpg) 好吧。光盘启动安装。让大家久等了。 注意看这个启动画面，多了一点信息。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f1c154fb828ba61efac552954b34970a314e5952.jpg) 这个Build的变化还是很多的。比如说，配置过程中不再询问是否连接网络（而是上来直接就装网络）——那个fdc.sys就是和网络安装有关系，不弄好就会导致在开始安装网络前卡住。此外安装程序也不会带你创建应急修复软盘了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f3efd750f819861891486f3e40ed2e738ad4e677.jpg) 这个Build里，设备管理器又从My Computer-&gt;Manage所能达到的这个界面消失了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/42fc1cf50ad162d94801eca61bdfa9ec8813cd97.jpg) 那么在哪里找呢？答案是，My Computer-&gt;Propertiles的Hardware选项卡。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/bdeb2635970a304e63805540dbc8a786cb175cdb.jpg) 设备管理器的驱动程序安装流程已经趋于Win2K RTM样式了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/1e2beab0cb1349543d4a61de5c4e9258d0094a2d.jpg) 另外，可以直接右击安装inf文件了\[真棒\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f20f24176d224f4aea51f9a903f790529a22d1b2.jpg) 许多大家所喜欢的附件也终于进入Accessories了。原来这个文件夹里没放入这些程序。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/79f5463eb80e7bec5b5df65b252eb93899506bfe.jpg) cghvbnc22:explorer，各向导又改了回去，关机后的屏幕喷\[吐\]\[喷\] 有一些备注：fdc.sys那个文件是肯定要弄的。是的，原来就有一个fdc.sys，必须把它用null.sys的副本替换。

至于如何替换，BWDB说要什么进安全模式弄。但是实际上进安全模式可能（由于Bug？）无法操作，进普通模式则会提示大概是“Access is denied”这样的信息——或许是我手速慢了一点。其实，大可以自己去搞张DOS启动盘或者PE镜像，到那里面定定心心弄。 仍然没有装上显驱。下面装1773。

Windows NT 5.0 Build 1773 阶段：Beta1 编译日期：1998年3月18日 版本字串：5.0.1729.1 winnt32的界面终于和重启后界面统一了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/cd45ac1249540923a8f92ac59858d109b1de49ea.jpg) 界面越来越成熟了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e1b0ca355982b2b79311707f3badcbef74099bf0.jpg) Safe Mode登场！（虽然我这儿用不到） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/0f36b2638535e5ddbbf8ec647cc6a7efcc1b62ae.jpg) 继续Debugging Mode。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/1b41aeeb15ce36d3fc95368b30f33a87eb50b1e9.jpg) 咦，怪了，BWDB和@cghvbnv22 都说这是Beta1，但是它认为自己是Beta2 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/0a649102738da977ef283290ba51f8198718e378.jpg) 仍然留着这个界面。“Last known good configuration”还没有被归到F5（后成为F8）那个界面。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e8279a1e4134970ab372a7949fcad1c8a6865d79.jpg) 又卡在这儿……不对升级抱希望了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e4fb2cfafbedab64be3cff7bfd36afc378311e30.jpg) CD启动。……空间需求真是水涨船高。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/6050212209f790529e83f58506f3d7ca79cbd5e6.jpg) 进PE换文件。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/65d9b32b2834349b1887d23ec3ea15ce34d3bef9.jpg) @cghvbnv22 这着实应该是Beta2吧！ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/20ad422cd42a28342d3689b051b5c9ea17cebfea.jpg) 上面一条的样子变了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/edc03e83b2b7d0a239d0ba26c1ef76094a369a61.jpg) 之前分两步的 设置Computer Name和密码 的过程，现在并一步了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/dc76b659ccbf6c81efb69253b63eb13531fa40f9.jpg) Workstation上不用再按Ctrl+Alt+Delete好评，登录界面更改好评。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/16baf559d109b3def6155dd3c6bf6c81820a4cdc.jpg) 右下角的徽标再次改动。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/7b33f83cf8dcd1003c1d409a788b4710bb122ff9.jpg) 磁盘管理。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/ed9abac551da81cba21f38765866d0160b243181.jpg) Logoff被归入关机选项。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f6093567d0160924345818a0de0735fae7cd3405.jpg) 安全模式启动时的信息稍不一样。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/61cbdf0f7bec54e7763ebfa5b3389b504dc26ab4.jpg) Safe Mode大赞！ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/750e81cc7b899e51abad9eaf48a7d933c9950d5b.jpg) 驱动继续装不上。装2K/XP的驱动，虚拟显卡不工作；装NT的驱动，出现了奇怪的错误。。。。。。真是叫人发火呐。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e3381bd88d1001e901eeb2b4b20e7bec56e797b4.jpg) Windows NT 5.0 Build 1796 阶段：Beta2 编译日期：1998年4月96日 版本字串：5.0.1796.1 1796的winnt32改放到了D:\i386\winnt32\。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/6d0187ff9925bc311add902354df8db1c91370fa.jpg) 不过Autorun.exe并不知情\[滑稽\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b227302d11dfa9ec5fbac7ac68d0f703938fc1ef.jpg) 在这里字体变了\[咦\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/9da0314f9258d109fc983a09db58ccbf6d814d03.jpg) 重启后。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/746f643a5bb5c9ea14869058df39b6003bf3b30d.jpg) 终于有开机画面了\[太开心\] 看这背景颜色，好像显驱终于在工作了？ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/bb06d5109313b07edac8c3b306d7912396dd8c0d.jpg) 系统色调更改。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b7c2c8c279310a5510684c4fbd4543a983261036.jpg) 哇，这次不仅没有出问题，VMware Tools还活着，并且还在帮我自动调节客户机分辨率\[惊哭\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c2f63daea40f4bfb61fc03ef094f78f0f6361856.jpg) 提示需要文件，叫我把CD插到D:，结果我放上镜像之后发现找不到D:\[啊\]感觉好紧张 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/327f2011b912c8fcb2396b76f6039245d48821bc.jpg) 看我搞点猛的。不是VMware Tools还在吗？我直接硬塞一个共享文件夹进去\[滑稽\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c722407e9e2f070890e7afbbe324b899ab01f2a5.jpg) 好不容易把那一段撑过去了，D:却在这时冒出来了\[喷\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d41a971e3a292df5cb3725aeb6315c6036a8738e.jpg) 启动时蓝屏会这样\[汗\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f86dce004c086e065be823f708087bf40bd1cb3b.jpg) 另外，虽然正常启动时只有开机动画，但安全模式还是有一些文字： ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d729c645ad3459822706f92e06f431adc9ef84f7.jpg) 这个Build为什么打不开explorer\[黑线\]我已经试了一下午了 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/7627b238b6003af3b897c3dc3f2ac65c1138b656.jpg) 足以安慰的是，这个Build从NT4升级算是成功了。经历了15xx~1729的那些麻烦，感觉还是1743好呀。有了显驱，连RA95都可以玩了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/5fc48e25b899a9010fcb448a17950a7b0008f581.jpg) 合照。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/ab30d04443a98226eb87359b8082b9014b90eb39.jpg) 由于尴尬地没有进入explorer，欢迎界面没有见到。太可惜了。大家可以到cghvbnv22的帖子去看看Welcome to Windows NT那个界面。 1796完\[高兴\] 然后……1835这个压缩包里不是镜像？！\[瞪眼\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/1976d5b6d0a20cf4a267e5637c094b36aeaf9988.jpg) 解压以后是\[心照不宣\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3deab51a0ef41bd55b9df2485bda81cb3bdb3db1.jpg) 再解压以后是这样\[暴躁\]镜像呢 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/678bf92e0708283826a1d9a8b299a9014e08f1d7.jpg) 弄了半天发现是给虚拟机用的。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e4fb2cfafbedab640d204e7cfd36afc378311e34.jpg) 呕，我吃完饭还没解压好\[喷\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/0fbe47a5462309f7deeaa6ae780e0cf3d5cad6fe.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/a9d0df98a9014c085ebe2319007b020879f4f4fe.jpg) 终于解压完了。还好是可以安装的。那么这个Build就可以发在这帖了。

Windows NT 5.0 Build 1835 阶段：Beta2（然而系统又把自己叫做RC0.2\[狂汗\]） 编译日期：1998年6月26日（禁毒日\[咦\]） 版本字串：5.0.1835.1 又是一个模样大改的Build。 看上去有些问题。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/cd45ac1249540923715413c29858d109b2de4946.jpg) 能升级NTFS好评。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4903f7539822720e46c4924671cb0a46f31fab7d.jpg) 看来本质上还是个Beta2。（重点错） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/9d3036db81cb39db531117eada160924a91830aa.jpg) ↑ 喂喂我这还怎么装，解压出来只有散装文件没得镜像，拿个i386文件夹手工做个镜像也不济事\[喷\]@cghvbnv22 好吧，幸亏我装Beta也是身经百战了（划掉），对付这种问题还行，刚才成功解决了问题。 怎么弄的呢？我先是把之前解压出来的i386文件丢进一个新建镜像里，发现系统不承认。 然后我对比看了看正常映像。其他有的Build镜像里也只有i386一个子文件夹，比我仅仅是映像根目录下多了两个文件（不同Build文件名不一样），但是它们都能正常安装。所以我就怀疑系统是认那两个文件的。我就从1796的镜像取出cdrom\_nt.5和cdrom\_w.5b1放进1835的自制映像里。没有成功。而后我从1877的镜像取出CDROM\_NT.5和CDROM\_IW.5B2两个文件放进1835的文件夹里。这一回成功了。 这个阶段重启后有新的壁纸。怒赞。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/678bf92e0708283807a1b8a8b299a9014e08f1d7.jpg) 重启后。现在这个启动界面的背景也统一为蓝色了。值得表扬的是那个蓝-白渐变的条子在1796尚不会动，在这个Build会动了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4a8f65097bf40ad1407ea05f5d2c11dfabecceed.jpg) 另一个进步： 1796还没有（至少应该是默认没有）鼠标指针的阴影 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c6ec517bdab44aed24a5de58b91c8701a38bfb9c.jpg)

但是1835有了 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d2acb608b3de9c82738499336681800a1bd8439a.jpg) 还有，MMC不再依赖于IE了。之前打开MMC会提示什么需要安装IE3以上（当然系统内置的IE5，怎么回事我不知道），现在不会了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/792fd1fc5266d016dfabfc949d2bd40737fa35d5.jpg) 设备管理器回归计算机管理。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/47fc4f391f30e924ac27fe8d46086e061f95f784.jpg) 由于一些小问题，tools没有自动打开。但是可以手动打开那个服务。这样VMtools就能开始工作，能帮你自动调客户机分辨率。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4fd025a6d933c89533a8f5c7db1373f0800200a9.jpg) 关机界面改为下拉菜单。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/89c917ce3bc79f3d4ee08a8cb0a1cd11738b297a.jpg) VGA mode收归F5界面了。（这一项倒是在1796做到的） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/750e81cc7b899e51d69c53a848a7d933c9950d75.jpg) 安全模式还是要显示一些字，但是字的颜色变了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/9a402dec2e738bd4b6fadb8dab8b87d6257ff9ac.jpg) 搜索驱动的位置多了一个Windows Update\[大拇指\]这大概是说明Windows已经要加入联网更新功能了吧。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f08aad8165380cd7ca35c951ab44ad345882815c.jpg) 其实刚才explorer还是没有正常运行→\_→我弄了这么久总改给我显示个Toolbar了吧。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/07e4de13c8fcc3ce7886a38f9845d688d53f2039.jpg) 还是没有 ![](http://static.tieba.baidu.com/tb/editor/images/client/image_emoticon72.png) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/678bf92e0708283816ac89a8b299a9014e08f1da.jpg) @asministator 刚才忍受不了没有explorer的糟糕体验，我全新安装了一遍并装了显驱。 Beta1的时候VM显驱都不工作，严重者蓝屏黑屏。到了Beta2就好了\[真棒\] 登录时桌面右下角的谜之徽标从此消失了\[升起\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d8d6150f0cf3d7ca654c79caf81fbe096963a9cd.jpg) 贴图好评。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/94cbe095a4c27d1e7f457b7811d5ad6edcc43824.jpg) IE5居然可以打开MSN门户，只报一个错\[吐舌\]百度主页可是要几十个的。可能是MSN门户使用的HTML新特性比较少吧。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/a6391c889e510fb3b6763f2bd333c895d0430c10.jpg) “关于”界面的IE徽标拖不动了。IE4的菜单已被移除\[不高兴\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/13b79cf3b2119313899ab60c6f380cd793238da2.jpg) 合照。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4f47682542a7d933d3e7cfcea74bd11372f00130.jpg) 1835完！\[玫瑰\] Windows NT 5.0 Build 1877 阶段：Beta2（又作RC0.2） 编译日期：1998年8月17日 版本字串：5.0.1877.1 继续调整UI。 多年不改的Autorun.exe ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/11fbbef8d72a605952a1fda72234349b013bbacb.jpg)

1848（SRV）开始缩水的安装界面\[吐\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/dba428c3d56285354ba8ce9c9aef76c6a6ef633c.jpg) 怎么又预感不妙\[啊\]（虽然系统伸手要驱动并不少见） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/8808a4cfc3fdfc0360f3fc05de3f8794a6c226fd.jpg) 还是没有桌面\[汗\]不得不从CD安装 这里的“Windows NT Workstation Setup”的“Workstation”被省去了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/cca0f3eff01f3a299a9ecf739325bc315d607c2a.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/ebecf02ad40735fae4924b0494510fb30e240825.jpg) 这里终于不用把条款拉到底才能按F8了\[笑眼\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/cb20d41d8701a18bb3b517f2942f07082938fe22.jpg) 现在CD启动不会出现这个界面了： ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/6e29c4cd7cd98d109821088c2b3fb80e79ec908f.jpg)

而只会显示： ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4903f7539822720e5187e54771cb0a46f31fab33.jpg) 安全模式还是这样。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4c07b0cb7bcb0a46abcd84846163f6246960af91.jpg) 正常启动后装了一下显驱。这里驱动安装界面还是稚嫩。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4cc7e045ebf81a4c0ce6e674dd2a6059272da6a8.jpg)

缩水的欢迎界面\[阴险\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f2e5f412b07eca801dac335a9b2397dda34483d3.jpg)

看新闻美滋滋\[滑稽\]（IE5 Beta似乎比IE5 RTM还好用，并且占用非常非常非常少） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/ed9abac551da81cbd31089705866d0160b24318a.jpg) 我记得OS Loader这个界面上，最开始没有“Starting Windows NT”，1835时方出现。1835的“Starting Windows NT”会显示在点的末尾，这里换了一行。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/8de5158a4710b9121ffb8243c9fdfc039345224e.jpg) 合照。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e3381bd88d1001e9756f5eb2b20e7bec55e79735.jpg) 既然NZJ很喜欢，我就把1888装一遍吧。 Windows NT 5.0 Build 1888（Server） 阶段：Beta2 编译日期：1998年9月4日 版本字串：5.0.1888.1 特此说明，1888目前只有Enterprise Server版，本来我没打算装。这里1888是在一堆Workstation里的一个例外，但又不是普通的Server，一些地方可能会比较特殊。 试图从NT4 Server升级。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/191a5a6c55fbb2fb9d7cc5af454a20a44723dc2a.jpg) 又出现这种状况了\[吐\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c7b08cf91a4c510f6e0931a76a59252dd62aa5b0.jpg) 因为有过经验，我上来就复制了1911的CDROM_IS.5B2和CDROM\_NT.5两个文件。很不幸，这次没有奏效。 幸好，文件名里的规律是容易发现的：1911的CDROM\_IS.5B2，IS的S代表Server，5B2代表NT5 Beta2。像1796里，相应地S变成了W，代表Workstation。不过为什么1796那个是.5B1，就说不大清楚了。——CDROM\_NT.5这个文件，每个Build里都是一样的。 那难道文件名对就行了吗？一般不是。但是我观察了一下，每个Build的CDROM_\*.5B\*和CDROM\_NT.5都只有几个字节大小；打开一看，并没有存储与版本信息相关的内容。那么这样的文件很可能只是起一个占位作用，可以直接挪用，只要文件名对了就行。 1888不是Server吗？CDROM\_NT.5显然不是问题的关键。为什么CDROM\_IS.5B2不行？我猜1888作为Enterprise Server是不是要把S换成E。我猜对了。 我就说1888会有什么特殊的地方，上面果然应验了\[惊哭\] 重启后。比WKS难看\[喷\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/79e6d41ab051f819e919daf7d0b44aed2f73e741.jpg) 这个界面不知何时起不再是一个窗口了。

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/2ef27a940a7b0208fc27e15c68d9f2d3552cc893.jpg) 楼上漏发这张了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4a8f65097bf40ad1ea561e5e5d2c11dfabecced7.jpg) 登录之前。

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/2c75e70b19d8bc3ea0d0df77888ba61eaad345ac.jpg) 好了不用说了，我又打不开explorer了 ![](http://static.tieba.baidu.com/tb/editor/images/client/image_emoticon72.png) 再从CD启动安装。 重启后……F5被F8替代了\[真棒\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/2dd6284b20a4462394637edf9222720e0ef3d7dc.jpg) 正常启动会卡在这儿\[怒\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f2e5f412b07eca80ad2be35a9b2397dda0448353.jpg) 所以我只好启动为安全模式。 安全模式的加载终于也脱离了NT4那种傻打印字到屏幕上方的样子，而是成为和后来一样的模样\[大拇指\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/ebecf02ad40735faa5f3940494510fb30e240805.jpg) 不论是不是安全模式，左下角的cmd又回来了\[咦\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/7625482fb9389b50ab8425ef8f35e5dde6116e0e.jpg) 正常启动和安全模式都装不冻\[泪\] 反正死猪不怕开水烫，我随便搞个Debugging Mode玩玩\[阴险\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/75dea15d10385343497fb29f9913b07ec88088d5.jpg) 开机界面和正常开机一样了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/8b1b11084b36acafeb5da24276d98d1003e99cc0.jpg) 你问我紧张不紧张，我是紧张的。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/745c39de8db1cb13a7ce08add754564e90584bda.jpg) 然后卡了我电脑一顿饭时间的关就这么容易地过去了\[喷\]我该说我运气好还是不好呢 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3b1833e636d12f2e691399de45c2d5628435686b.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/25cc6bd6912397dd18f8afba5382b2b7d2a28784.jpg) 不好了，又滞留在这儿了\[心碎\]难道这个Build开了历史的倒车，又要折腾fdc.sys了\[怒\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/ef371e300a55b319a391b4cb49a98226cefc171c.jpg) 还好只是虚惊一场\[呼~\]幸好没有匆忙重启 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/38049037afc379314cc1b097e1c4b74541a911d3.jpg) 耶！ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/91f4dda0cd11728b551ebd9cc2fcc3cec2fd2c55.jpg) 诶？ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c2f63daea40f4bfbc5caafea094f78f0f636186e.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c2f63daea40f4bfbc546afea094f78f0f53618ea.jpg) 不管它了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/6e87ecd5b31c8701fff982582d7f9e2f0608ff32.jpg)

Server的Welcome缩水更多\[汗\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/17d876dea9ec8a131618675efd03918fa1ecc007.jpg) 照管理上显驱。 终于分出Driver Details、Uninstall、Update Driver三个按钮了\[真棒\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4a2505d8f2d3572c6305ac628013632760d0c39a.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/75dea15d1038534350bdb59f9913b07ecb808817.jpg) 尽给我搞事情\[喷\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c13f5edab6fd5266f40401aaa118972bd5073651.jpg) 还好重启后就好了\[开心\] ——我明明在安装的时候把所有可选组件都去掉了，结果游戏还是装了上去\[汗\]Windows 2000 Server的这几个游戏一直保留到SP4 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d2acb608b3de9c823dacc7316681800a1bd843bc.jpg) 合照。——Workstation搞啥\[喷\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c7b08cf91a4c510f5093c3a46a59252dd52aa52a.jpg) 瞎改了改系统图标……感觉自己好逗比。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/01c0f00b304e251f720df146ad86c9177d3e538f.jpg) 1888完。 Autorun仍然找不到Winnt32\[弱\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/768ebdb54aed2e73c78ba7938d01a18b86d6fa20.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/bcf7f544d688d43f8cedb04d771ed21b0ff43b39.jpg) 手动选择重启变成了15秒自动。但是我不喜欢\[汗\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/411d5e00213fb80ec2b941683cd12f2eb838941e.jpg) 驱动安装这一小步变得相对独立了些。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/6050212209f79052ef48648106f3d7ca7acbd52b.jpg) 在RAMDisk足够快的情况下，安装设备已经成了安装过程中最慢的一步了。不过这也侧面反映出随着系统的进步，其他地方已经不大会再出岔子耽搁时间了。 不过出现了看着有点吓人的情况。幸好不是大事。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/8be72e550923dd548c158ad7db09b3de9d824824.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e6eacfd2fd1f41347b8628c12f1f95cad3c85ed5.jpg) 艾玛这里动不了鼠标和键盘了\[惊哭\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/0bc2cbae2edda3ccd34a949f0be93901233f92dc.jpg) 虽然说F8已经投入使用，但是F5还没有被取缔： ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d7dfb30635fae6cd61f587de05b30f2440a70fc4.jpg) （恢复快照）唰！时光倒流。 是不是我这里懒得装VMware的驱动导致的问题\[思考\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/11fbbef8d72a6059a0a4cfa52234349b013bbaca.jpg) 忘了说了。这里安装开始菜单项目这个芝麻大点事被单独立出来了\[汗\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/9a402dec2e738bd4f6e09b8eab8b87d6257ff945.jpg) 还是不来事。你想跟我说启动失败的是键鼠驱动吗\[阴险\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/fccad63433fa828b4574b55cf71f4134960a5a2b.jpg) 1902好像不怎么好启动\[狂汗\]（卡在这个界面） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e8279a1e4134970a90a940909fcad1c8a5865da8.jpg) 还是用DOS安装吧…… 顺手试了下，winnt /ox还是可以用的。不截图了。 这个好智能\[滑稽\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d729c645ad345982e795b92d06f431adcaef8463.jpg) 启动成功。（\*上面一个选项是原来的DOS） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f3efd750f8198618d697a63b40ed2e7389d4e6b7.jpg)

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/86a877395343fbf289e4eb9cba7eca8067388fbe.jpg) 装好之后。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/11fbbef8d72a605907e1aaa52234349b013bba95.jpg) 玩腻了平常的驱动安装。试试自动搜索。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/553a51d2d539b6001002bb08e350352ac45cb7b2.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/fefd0c62f6246b601bca06cbe1f81a4c530fa2ba.jpg) 好像搜对了？ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e9f52b096e061d95e49f808771f40ad160d9caae.jpg)

噫…… ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/70ba421e95cad1c820a44b98753e6709c83d5163.jpg) 再来一次。搜到了什么有趣的东西。（D:是这个系统安装根目录） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/1976d5b6d0a20cf40e3149607c094b36aeaf99e5.jpg) 安装后。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/22249002918fa0ecf521d3b22c9759ee3f6ddba5.jpg) 这回成功了？！ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3c2dea1101e9390169533c8171ec54e737d19635.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/bd0ec850f3deb48fd13e1161fa1f3a292cf5782b.jpg) 楼上丢失的图片是： ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/9596e234e5dde711c471f349adefce1b9f1661e7.jpg) 只要作极小的修改，1902和NT4几乎完全一致的。你们看看这张截图，要是不看winver，你能看出和NT4有什么区别么\[滑稽\] 提示：除winver仅有两处不同。@xkai 你能看出来吗\[滑稽\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/7add4af4e0fe992594ff9df23ea85edf8fb17192.jpg) 合照。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/49d7ba55564e9258ff90754c9682d158cebf4ee5.jpg) Windows NT 5.0 Build 1906 阶段：Beta2 编译日期：1998年10月7日 版本字串：5.0.1906.1 这个Build开始，CD目录下多出了很多东西。 CD根目录下。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/17d876dea9ec8a13cc6aa942fd03918fa1ecc012.jpg) advsetup里包含了一些有趣的信息，如：

## Using Command Line Parameters

You can customize the way Setup performs by using any of the following command line parameters. Winnt.exe Command Syntax The syntax of the Winnt command is as follows: WINNT \[/S\[:sourcepath\]\]\[/T\[:tempdrive\]\]\[/I\[:inffile\]\] \[/X\]\[/F\]\[/B\]\[/C\]\[/U\[:answer file\]\]

where:

* /A enables Accessibility options.
* /B skips the creation of the Setup startup floppy 

  disks. Instead, the command creates a disk image of the 

  floppy disks, which can be used after Setup restarts 

  the computer.

* /C skips the free space verification of the Setup 

  startup floppy disks.

* /E specifies a command to be executed at the end of 

  GUI-Mode Setup \(that is, after your computer has 

  restarted twice and after Setup has collected the 

  necessary configuration information, but before Setup 

  is complete\).

* /F skips the file verification step as files are 

  copied to the Setup startup floppy disks.

* /I\[:inffile\] specifies the file name \(no path\) of the 

  Setup information file. The default file name is 

  Dosnet.inf.

* /Ox creates Setup startup floppy disks for installation 

  from a CD.

* /R specifies optional folder to be installed. The 

  folder remains after Setup finishes.

* /Rx specifies optional folder to be copied. The 

  folder is deleted after Setup finishes.

* /S\[:sourcepath\] specifies the source location of the 

  Windows NT files. The location must be a full path of 

  the form x:\[path\] or \server\share\[\path\]. The default

  is the current folder. To simultaneously copy files 

  from multiple servers, you need to specify multiple 

  /S sources.

* /T\[:tempdrive\] specifies a drive to contain temporary 

  Setup files. If you don't specify a location, Setup 

  attempts to locate a drive for you.

* /U\[:answer file\] performs unattended Setup using 

  optional answer file \(

  requires /S\). The answer file 

  provides answers to some or all of the prompts the end 

  user normally responds to during Setup.

* /X skips the creation of the Setup startup floppy 

  disks. The Setup startup floppy disks that came with 

  your Windows NT software are required after Setup 

  restarts the computer.

Winnt32.exe Command Syntax The syntax of the Winnt32 command is as follows: winnt32 \[/s:sourcepath\] \[/tempdrive:drive\_letter\] \[/unattend\[num\]\[:answer\_file\]\] \[/copydir:folder\_name\] \[/copysource:folder\_name\] \[/cmd:command\_line\] \[/debug\[level\]\[:filename\]\] \[/udf:id\[,UDF\_file\]\] \[/syspart:drive\_letter\]

where:

* /copydir:folder\_name creates an additional folder 

  within the folder that contains the Windows NT files. 

  For example, if the source folder contains a 

  Private\_drivers folder that has modifications just for 

  your site, you can type /copydir:Private\_drivers to 

  have Setup copy that folder to your Windows NT folder

  \(for example, C:\Winnt\Private\_drivers\). You can use 

  the /copydir option to create as many additional 

  folders as you like.

* /copysource:folder\_name temporarily creates an 

  additional folder within the folder that contains the 

  Windows NT files. For example, if the source folder 

  contains a Private\_drivers folder that has 

  modifications just for your site, you can type 

  /copysource:Private\_drivers to have Setup copy that 

  folder to your Windows NT folder and use its files 

  during Setup \(for example, C:\Winnt\Private\_drivers\). 

  Unlike folders created by the /copydir option, folders 

  created by using /copysource are deleted after Setup 

  completes.

* /cmd:command\_line instructs Setup to carry out a 

  specific command before the final phase of Setup \(that 

  is, after your computer has restarted twice and after 

  Setup has collected the necessary configuration 

  information, but before Setup finishes\).

* /debug\[level\]\[:filename\] creates a debug log at the 

  level specified. The default creates a log file 

  \(C:\Winnt32.log\) that has the level set to 2 \(Warning\).

* /s:sourcepath specifies the location of the 

  Windows NT files. To simultaneously copy files from 

  multiple servers, you need to specify multiple /s 

  sources.

* /syspart:drive\_letter specifies that you can copy Setup

  startup files to a hard drive, mark the drive as active,

  and then install the drive in another computer. When 

  you start that computer, Setup automatically starts with

  the next phase. You must always use the /tempdrive 

  parameter with the /syspart parameter.

* /tempdrive:drive\_letter directs Setup to place 

  temporary files on the specified drive.

* /unattend upgrades your previous version of 

  Windows NT in Unattended mode. All user settings are 

  taken from the previous installation, so no user 

  intervention is required during Setup.

* /unattend\[num\]:\[answer\_file\] performs a fresh 

  install in Unattended mode, using an answer file for 

  user settings. 

Num is the number of seconds between the time that Setup finishes copying the files and the time Setup restarts. You can use the num option only on a computer running Windows NT. Answer\_file is the name of the answer file. For more information about answer files, see the Windows NT 5.0 Deployment Guide.

* /udf:id\[,UDF\_file\] indicates an identifier \(id\) that 

  Setup uses to specify how a Uniqueness Database File 

  \(UDF\) modifies an answer file \(see the /unattend entry\).

  The UDF overrides values in the answer file, and the 

  identifier determines which values in the UDF file are 

  used. For example, /udf:RAS\_user,Our\_company.udf 

  overrides settings specified for the identifier 

  RAS\_user in the Our\_company.udf file. If no UDF\_file is

  specified, Setup prompts the user to insert a disk 

  that contains the $Unique$.udf file.

  这是什么奇葩的拒绝理由\[喷\]

  ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/0a1949728bd4b31c129c6c198dd6277f9c2ff8e2.jpg)

  害得我把整个光盘的内容拷进了虚拟机硬盘，然后把EULA拷进winnt32\。

  ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/90e26e25ab18972bb66bfb68eccd7b899f510a30.jpg)

  照样不行\[心碎\]

  ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/2dd6284b20a44623b4c15ec09222720e0df3d77b.jpg)

  最后是把winnt32\的所有文件复制到i386\下，再运行i386\里新拷进的winnt32.exe这才行。

  ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/fefd0c62f6246b60c5bb48d6e1f81a4c530fa2d5.jpg)

  安装过程中有驱动缺失时默认到本地硬盘去找而不是要光盘了。

  ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/327f2011b912c8fc85cd106ff6039245d788214f.jpg)

  ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/bcf7f544d688d43fcbed7750771ed21b0cf43bc5.jpg)

  再度动不了鼠标。不得已从光盘启动安装。这里怎么就能看到用户协议呢。 

  ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c7f5c68a87d6277f1314de9a22381f30e824fc00.jpg)

  在这里，进度条一下越到末尾，我就觉得不正常，因为平常安装设备这里怎么也要好几分钟的。果不其然，后来在这里卡了十多分钟。

  ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/8eeffa17fdfaaf51f63b6f1d865494eef21f7aa9.jpg)

  强行重启，进入Debugging Mode。不知道为啥Debugging Mode常常可以解决一些NT5预览版的玄学问题。

  图片已经说明是Beta3了？！

  ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/792fd1fc5266d0164635758a9d2bd40734fa355d.jpg)

  看上去正常了一点。

  ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b7c2c8c279310a55df393556bd4543a98326106c.jpg)

  用那个cmd开winver，看到了奇怪的注册人\[滑稽\]

  ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c5c182dce71190ef8a3e797dc41b9d16fffa6045.jpg)

  regsvr32不知道什么时候上线了。之前敲regsrv32还提示不存在。

  ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/a9a4522bc65c103883971a60b8119313b27e8999.jpg)

  那注册个mmcndmgr.dll玩玩。如果不注册这个dll，就不能在安装阶段打开MMC了。

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/fefd0c62f6246b60b5c458d6e1f81a4c530fa244.jpg) ？ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/bd0ec850f3deb48f8e36747cfa1f3a292cf5782e.jpg) ？？ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/68cc7831e924b89925a0ac9a64061d95087bf6ee.jpg) ？？？ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/90e26e25ab18972b9b00d468eccd7b899f510a4b.jpg) 。。。 感觉不妙，这里又是滞留了十几分钟了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/89e3183f6709c93d5bded855953df8dcd000545d.jpg) 只能再试试Safe Mode了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4903f7539822720ea7d6335871cb0a46f31fab6a.jpg) 还是DOS安装的能用。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/768ebdb54aed2e73fb4b438e8d01a18b85d6faec.jpg) 16色终于不那样硬要模仿真彩色了，变得质朴了一些\[真棒\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/2c75e70b19d8bc3eba97c168888ba61eaad345ee.jpg) 粗体字有点难看。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/1c9453a95edf8db137a1bbc60323dd54544e74ff.jpg) 安装过程顺利，不提。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/92ef69f51bd5ad6e5731cd4e8bcb39dbb4fd3cbb.jpg) 破炸弹后的合照。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/47fc4f391f30e924748a369546086e061c95f75a.jpg) Windows 2000 Build 1946 阶段：Beta3 编译日期：1998年12月13日 版本字串：5.0.1946.1 NT5.0终于蜕变成了2000！\[花心\] NT 5.0变成2000好评，Workstation全部变成Professional好评，Autorun.exe变成Setup.exe并改进界面好评，CD下目录被整理过好评，Bootdisk出现好评…… ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c2d2a8fd1e178a8239a09804fc03738dab77e8e8.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/592cdb3fb13533faaf5f748aa2d3fd1f43345b9a.jpg)

不过条款尚未更改称呼。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/678bf92e07082838892f3ab0b299a9014d08f16e.jpg)

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/94de4f35349b033b89a21a7e1fce36d3d439bd66.jpg) 启动选项界面也有个“NT5”没有改。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/94de4f35349b033b89191a7e1fce36d3d739bdf3.jpg) 哎呀，这里卡住了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/cb20d41d8701a18b1678f4eb942f07082a38fefd.jpg) Debugging Mode？ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c2d2a8fd1e178a82c6d89904fc03738dab77e8a0.jpg) 实践发现，Safe Mode、Debugging Mode都不行。 CD启动？ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d0a6ff23720e0cf36b00af5f0046f21fbc09aa91.jpg) 依旧不行。 难道逼我使出DOS？ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b7f7f68ea0ec08fafa3ef30353ee3d6d54fbda4a.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/91fdd4df9c82d158ef8bb9158a0a19d8bd3e427a.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/222d95d2572c11df0a375f87692762d0f503c2a2.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/edbfb61273f0820230ba719b41fbfbedaa641b5b.jpg) lz目前还没有解决问题。可能要明天才能弄出来了。 之前我关和不关ACPI试下来都不行\[狂汗\] 不过我真是傻，1946镜像里已经有CDBOOT1.img等4个启动软盘的映像了，直接从iso里拿出来就能启动了。 软盘启动的。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c0fe7ed9bc3eb135c5978a1dac1ea8d3fc1f443d.jpg) F1打开帮助的功能不见了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/13b79cf3b21193131ddbc2166f380cd793238df5.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/49d0cc19972bd4071de2ef5b71899e510eb30967.jpg) WTF？！ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/833aa4fcfc039245c2d0dda98d94a4c27c1e2527.jpg) 没办法，这真是跟1386一样难装了。不，或许甚至还要胜过一筹。1386要是成功搞到启动软盘可能就直接启动了，只不过当时懒得用软盘而已。 那么我只能这么装： 1.从DOS启动安装1946，复制完文件后提示按ENTER重启继续的时候，不按ENTER重启，而是关机。 2.映射虚拟磁盘，把根目录:$WIN\_NT$.~LS下的所有内容拷出来。 3.从DOS启动安装另一个NT5 Build，复制完文件后提示按ENTER重启继续的时候，不按ENTER重启，而是关机。 4.可写映射虚拟磁盘，把根目录:$WIN\_NT$.~LS下的所有内容删了，然后把1946的相应文件拷进去。 5.开机，从硬盘启动安装。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/746f643a5bb5c9ea8d0b3945df39b60038f3b395.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c27fc11fa8d3fd1fb23c879c3a4e251f94ca5f50.jpg)

哎呀，依然不行。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f1c154fb828ba61e5a11f2894b34970a324e598a.jpg) 又把$WIN\_NT$.~BT也弄进去了。 还是不行\[泪\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/03e20a234f4a20a43e071b619a529822730ed074.jpg) 可能是我用的“另一个NT5 Build”和1946差得太远了吧。再用1983替代，结果1983自己又不能启动\[惊哭\]难道Beta3起要有好长一段难熬的时光了 真是的,我一把硬件兼容性改成VMware Workstation 5.x,虚拟机马上丝滑流畅。新版VM对老系统的兼容性不够好。 录播。 不出所料，F1还是在的，只是软盘启动没有而已。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/75dea15d10385343be2bdf879913b07ec88088a1.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e1b0ca355982b2b780c663623badcbef77099b34.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f08aad8165380cd7dd92fa4bab44ad345b8281f9.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4c0056accbef76091cbec13924dda3cc7ed99ed0.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/79e6d41ab051f81968445becd0b44aed2f73e72d.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d53eb6c9a786c917e18b0a9fc33d70cf39c75785.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/750e81cc7b899e51c76262b248a7d933ca950d99.jpg) Windows 2000和NT5字样并存。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/79e6d41ab051f81968cd5becd0b44aed2c73e7a6.jpg) 换了图片的开机界面，还是挺淡雅的\[真棒\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/25cc6bd6912397ddea2adda25382b2b7d1a2873e.jpg) CMD还在……

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/6050212209f7905285a6029806f3d7ca79cbd5d4.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/222d95d2572c11dfa182fa85692762d0f603c23e.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/07e4de13c8fcc3ce696e8c959845d688d63f20db.jpg) 好吧还是没有全部改掉……还把自己叫作Windows NT。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d7fe574f251f95ca4925d710c3177f3e650952bd.jpg) 任务管理器的名称“Windows NT Task Manager”中“NT”被删除了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e6eacfd2fd1f4134039e40d82f1f95cad3c85ee4.jpg) 雾草正在安装1946的这个时候还能安装1946，而且还是升级\[喷\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/bb19cc65034f78f0219bdf5573310a55b1191cfd.jpg) 。。。我好无聊 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/553a51d2d539b60001b14a11e350352ac75cb70a.jpg) 这些启动项有点乱233 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/9a402dec2e738bd45ec0f397ab8b87d6257ff9ad.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/91e714f182025aaf6940386df1edab64024f1a1f.jpg)

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/2dd6284b20a446231196e3c49222720e0df3d729.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/94de4f35349b033b693eba7c1fce36d3d739bdd3.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/bdeb2635970a304eaa06e25cdbc8a786c8175c61.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/327f2011b912c8fc61ebb46bf6039245d7882175.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/13b79cf3b21193138e1fbd166f380cd790238d29.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/bb06d5109313b07e8a5813ae06d7912395dd8ca0.jpg) 装上显驱以后那个清爽呀。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f9e6affdc3cec3fd5ebbebd3dc88d43f85942780.jpg) 简洁的壁纸\[真棒\]\[爱心\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/7a738e51352ac65c266729d5f1f2b21192138a2f.jpg) 不过窗口标题栏的颜色不那么好看了\[不高兴\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/553a51d2d539b60009f84211e350352ac75cb753.jpg) 合照。 Windows 2000 Professional字样、图片好评。注册表谜之键值HKEY\_DYN\_DATA彻底消失。IE5的“关于”界面更易，徽标再也不让人感觉好像使点劲就能拉动。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4ab2951ebe096b63ed1710f606338744eaf8ac7b.jpg) 这里还有“Workstation”\[汗\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/65ebf2cbd1c8a786ad02d9a96d09c93d71cf5066.jpg) 现在玩CS，不会因为鼠标滚轮支持问题难以换枪了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/91e714f182025aaf3d01ec6cf1edab64024f1a5f.jpg) Windows 2000 Build 1965 阶段：Beta3 编译日期：1999年1月22日 版本字串：5.0.1965.1 这回又是散装文件\[鄙视\] 手动包装了个镜像。放进虚拟机一看，又是什么都有，就缺个winnt32\[喷\]我表示强烈抗议 又手动给镜像加了个cdrom\_ip.5b3，这样做出的光盘镜像是能认，但启动失败。 还得用DOS\[泪\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/68cc7831e924b8990b71869f64061d950b7bf63a.jpg) 忘了说了，在真彩色下打开这个Build的winnt.exe，颜色有点点不一样\[咦\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f1c154fb828ba61e9f3937884b34970a324e59b3.jpg) 呼~ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/eb90644e78f0f736c4eba5a60055b319eac41371.jpg) 下方变成“Windows 2000”好评。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/43bb1ff1f736afc32cfef9c2b919ebc4b5451298.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/9da0314f9258d109b2246815db58ccbf6e814d43.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d7fe574f251f95cac2fe5211c3177f3e66095207.jpg) 这个图片好像是新的。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e0186ffb513d2697d4d5c8fa5ffbb2fb4216d80d.jpg) 继续亲民。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/7159acee76094b367d43da4aa9cc7cd98f109dbe.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/03e20a234f4a20a4d311fc609a529822730ed004.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/0a649102738da9775b97468cba51f8198418e3d7.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4a8f65097bf40ad11d5e07445d2c11dfabecced1.jpg) 自动登录！！ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/112ee6ca39dbb6fd643d25810324ab18962b372c.jpg) 图标改变好评。然而那张壁纸不见了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3304e5035aafa40f00be0d7aa164034f79f01916.jpg) 缺了一块是什么鬼啦。注意，“Workstation”变成“Computer”了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f9f52d91f603738dc916cf85b91bb051f919ec2b.jpg) Banner（当然做壁纸是有点奇葩）还显示是1998年，虽然这个Build已经是1999的了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/11c9419659ee3d6ddb2e446c49166d224d4adea7.jpg) cmd开始自称Windows 2000并显示详细版本好评。IE版本号2013。。。其他没什么了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/bb06d5109313b07e77ae9caf06d7912396dd8c78.jpg) “Welcome to Windows 2000”变成了“Get Started with Windows 2000”。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c760c3c37d1ed21b267be042a76eddc453da3fd8.jpg) 这个Build有个Bug：如果你没有设置账户密码，那么注销的时候，把程序全部关闭以后，系统根本不给你选择登录到的账户，而是直接再自动登录回你注销前的账户。这样你就没法切换用户了\[喷\] 1965完。我下载到的1969解压出来文件损坏不能用，暂时弄不了。 感谢 兰兰和随随 指出，1965是有winnt32的。我试着进行了升级安装。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e772ae167f3e6709ca437a5631c79f3dfadc55c8.jpg) 许可条款还是NT5的。

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/75dea15d103853435291bb889913b07ecb808836.jpg) 不过很遗憾，这里依然卡住，不论是否开ACPI、采用安全模式，都不能启动。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e3381bd88d1001e9f9202aa6b20e7bec55e79774.jpg) 又到Workstation 5.x兼容性的一台虚拟机里装了NT再升级到1965。这样就没有问题。VM你到底是怎么回事\[喷\] 有一点我之前没说：1965的这个地方把“Professional”去掉了： ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/47fc4f391f30e924e942b39846086e061f95f7ae.jpg) 但这个地方还没去掉…… ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f3e8e000a18b87d66de085b60d0828381d30fdea.jpg)

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/86a877395343fbf22be9898aba7eca8067388f43.jpg) 下面会不会中途出问题只能听天由命了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3deab51a0ef41bd5a724c65d5bda81cb38db3d1c.jpg) 成功升级\[钱\] 不过程序升上来了，驱动反而没了是几个意思\[喷\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/6fdade399b504fc260e4a5acefdde71192ef6dd1.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/7159acee76094b3609530e44a9cc7cd98f109d4f.jpg) 还好能装得上。——自动登录没有开启\[咦\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/8f0879168a82b901782cd79a798da9773b12ef8f.jpg) 升级时把tools带到有的NT5/2K Build里，会导致虚拟机异常，甚至整个VMware异常。 但是1965与VMware Tools相处得特别好\[真棒\] 如图，虚拟机可以自动适应窗口大小，能够调整到任意分辨率。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4c0056accbef7609eb44883624dda3cc7ed99ec5.jpg) 对，调得很小也可以…… ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b7c2c8c279310a55964dce5dbd4543a983261026.jpg) 最好的是，还能拖拽文件！\[真棒\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/678bf92e070828385a65cdbdb299a9014d08f120.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/0b0f9cecab64034f5871d2afa5c3793108551dcb.jpg) 我先装1969了。 Windows 2000 Build 1969 阶段：Beta3 编译日期：1999年1月29日 版本字串：5.0.1969.1 感谢 兰兰和随随 提供安装文件。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3b3f6d47f21fbe09aafc22be61600c338544adf4.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/8808a4cfc3fdfc03da180212de3f8794a5c22629.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b0eb5d282df5e0fe8dbc68ab566034a85cdf72ed.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/6fdade399b504fc2d4fd51afefdde71192ef6deb.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/bd0ec850f3deb48f82d34074fa1f3a292ff578d3.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f32afb83d158ccbf491b549013d8bc3eb33541ee.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/fefd0c62f6246b60c86e53dee1f81a4c500fa22a.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/7add4af4e0fe9925a97888fa3ea85edf8cb1711d.jpg) 安全界面六个按钮位又凑全了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/68cc7831e924b8992bc1a69264061d95087bf695.jpg) 合照。——IE为什么没有被升级\[喷\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/23d305d1f703918f3255e4605b3d26975beec48e.jpg) 1965这里还有Starting WIndows NT， ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f86dce004c086e069ddfe5e108087bf40bd1cb1f.jpg)

1969没了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/03e20a234f4a20a4dcc4f96d9a529822700ed0bc.jpg) Windows 2000 Build 1983 阶段：Beta3 编译日期：1999年2月18日 版本字串：5.0.1983.1 Win2K RTM化更深了。（废话） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b32ad38e8c5494ee1ea2ccb327f5e0fe9b257e8a.jpg) \[弱\]\[喷\]这还找不到 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/61cbdf0f7bec54e7ecbdd9b4b3389b504ec26a39.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3c2dea1101e93901f7444e9471ec54e734d196c8.jpg) EULA更新好评。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/1c9453a95edf8db13368bfce0323dd54544e74c8.jpg) .更新后的EULA：

MICROSOFT LICENSE AGREEMENT for Microsoft Windows 2000 Professional Pre-Release Code

\(c\)1999 Microsoft Corporation. All rights reserved.

This is a legal agreement \(""Agreement""\) between you \(either an individual or an entity\), the end user \(""Recipient""\), and Microsoft Corporation \(""Microsoft""\). BY INSTALLING, COPYING OR OTHERWISE USING THE PRODUCT \(AS DEFINED BELOW\), YOU AGREE TO BE BOUND BY THE TERMS OF THIS AGREEMENT. IF YOU DO NOT AGREE TO THE TERMS OF THIS AGREEMENT, DO NOT INSTALL, COPY OR USE THE PRODUCT. THIS SOFTWARE IS TIME SENSITIVE AND WILL NOT FUNCTION AFTER 300 DAYS FROM THE DATE IT IS FIRST INSTALLED.

1. GRANT OF LICENSE. 

\(a\) Microsoft grants Recipient a limited, non-exclusive, nontransferable, non-assignable, royalty-free license to install and use copies of the software accompanying this agreement \(the ""Product""\) on a maximum of five \(5\) computer’s residing on Recipient's premises, solely for Recipient’s internal testing. All other rights are reserved to Microsoft. Recipient shall not rent, lease, sell, sublicense, assign, or otherwise transfer the Product or any accompanying printed materials \(""Documentation""\). Recipient may not reverse engineer or decompile the Product, except to the extent that local law expressly prohibits the foregoing restriction. Recipient may not use the Product in a live operating environment where it may be relied upon to perform in the same manner as a commercially released product or with data that has not been sufficiently backed up. Recipient may not use the Product for benchmark or performance testing. Microsoft and its suppliers shall retain title and all ownership rights to the Product, and this Agreement shall not be construed in 3. SUPPORT. Microsoft is not obligated to provide technical or other support for the Product. However, limited technical support \(""Support Services""\), if noted in the materials provided to Recipient by Microsoft, may be available. Use of any such Support Services is governed by the Microsoft policies and programs described in ""online"" documentation, and/or in other Microsoft-provided materials. Any supplemental software code provided to Recipient as part of the Support Services shall be considered part of the Product and subject to the terms and conditions of this Agreement. With respect to technical information Recipient provides to Microsoft as part of the Support Services, Microsoft may use such information for its business purposes, including for product support and development. Microsoft will not utilize such technical information in a form that personally identifies Recipient. Such limited Support Services may not be available in all countries outside the United States and will be discontinued once the Product is commercially released.

1. MAINTENANCE. Microsoft is not obligated to provide maintenance,

   technical support, or updates to Recipient for Product licensed 

   under this Agreement. In no event shall Microsoft be obligated

   to provide Recipient, free of charge, a copy of the commercial 

   release version of the Product in connection with Recipient’s 

   participation in the testing program. Microsoft is not obligated

   to make the Product commercially available. 

2. CONFIDENTIALITY. The Product, including its existence and 

   features, are proprietary and confidential information to MS and 

   its suppliers. Recipient agrees not to disclose or provide any of 

   the Product, documentation, or any information relating to the 

   Product \(including the existence of the Product, features, or the 

   results of use or testing\) to any third party

3. LIMITATION OF LIABILITY AND REMEDIES. Notwithstanding any damages

   that you might incur for any reason whatsoever \(including, 

   without limitation, all damages referenced above and all 

   direct or general damages\), the entire liability of Microsoft 

   and any of its suppliers under any provision of this Agreement 

   and your exclusive remedy for all of the foregoing shall be 

   limited to the greater of the amount actually paid by you for 

   the Product or U.S.$5.00. The foregoing limitations, exclusions

   and disclaimers shall apply to the maximum extent permitted by 

   applicable law, even if any remedy fails its essential purpose.

4. GOVERNING LAW; ATTORNEYS’ FEES. This Agreement shall be construed

   and controlled by the laws of the State of Washington, and 

   Recipient consents to the jurisdiction and venue in the

   federal courts sitting in King County, Washington, unless no 

   federal subject matter jurisdiction exists, in which case 

   Recipient consents to the jurisdiction and venue in the Superior

   Court of King County, Washington. Recipient waives all defenses

   of lack of personal jurisdiction and forum nonconveniens. Process

   may be served on either party in the manner authorized by 

   applicable law or court rule. If either Microsoft or Recipient 

   employs attorneys to enforce any rights arising out of or relating

   to this Agreement, the prevailing party shall be entitled to 

   recover reasonable attorneys' fees.

5. U.S. GOVERNMENT RESTRICTED RIGHTS. The Product and Documentation 

   provided to the U.S. Government pursuant to solicitations issued 

   on or after December 1, 1995 is provided with the commercial 

   rights and restrictions described elsewhere herein. Product and

   Documentation provided to the U.S. Government pursuant to 

   solicitations issued prior to December 1, 1995 is provided with

   RESTRICTED RIGHTS as provided for in FAR, 48 CFR 52.227-14 

   \(JUNE 1987\) or F

   升级就卡在了这儿\[汗\]

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3b1833e636d12f2e70b592cb45c2d562873568da.jpg)

   CD启动后。

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/1e2beab0cb134954eeaed4cf5c4e9258d3094ada.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/6fdade399b504fc219b88caeefdde71192ef6daf.jpg)

   糟糕。

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c0fe7ed9bc3eb135c6778b10ac1ea8d3ff1f44da.jpg)

   新建了个虚拟机，把硬盘设置成IDE，问题解决。

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4c23f62297dda1441faf5319b8b7d0a20ef486e8.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d41a971e3a292df53d5193beb6315c6036a87384.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b32ad38e8c5494ee2a6d30b227f5e0fe9b257ec7.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f243b7a30cf431ad73647c924136acaf2cdd98d8.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f32afb83d158ccbf830a8a9113d8bc3eb33541d8.jpg)

   “OS Loader 5.0”消失。

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/1292b7170924ab18b2b0de9c3ffae6cd79890bef.jpg)

   RTM式开机画面。但是我个人觉得还不如Beta3。。。

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/0b0f9cecab64034f4323fdada5c3793108551da7.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/9a402dec2e738bd4e4ac8d9aab8b87d6257ff985.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/5d616d7a02087bf463a26842f8d3572c13dfcfc0.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/0f36b2638535e5dd464aa7747cc6a7efcf1b6228.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/990db02b6059252d44ed39af3e9b033b59b5b99c.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/42fc1cf50ad162d9cc0760b71bdfa9ec8813cda1.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3b006dd062d9f2d368f82644a3ec8a136127cca1.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e6eacfd2fd1f4134650d22d52f1f95cad0c85e5c.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f47beb5594eef01f94b81a6eeafe9925be317de6.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4a2505d8f2d3572c510b9e778013632760d0c3a1.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/cb20d41d8701a18bd5e935e4942f07082938fe14.jpg)

   年份用两位数表示，差评。

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/8808a4cfc3fdfc0377c3e113de3f8794a6c226d3.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d01b11c7a7efce1b393ec461a551f3deb58f657d.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f243b7a30cf431ad42fd4f924136acaf2fdd9867.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/27fdae3c70cf3bc74769c047db00baa1cc112a21.jpg)

   banner有所变化。

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d7dfb30635fae6cd8329a5ca05b30f2440a70ff5.jpg)

   合照。——IE开始拥有状态栏。

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/1976d5b6d0a20cf4b77af0747c094b36aeaf99ac.jpg)

   好不容易装上了虚拟声卡驱动，我试着播放音乐。

   居然可以想办法开两个WMP\[喷\]把同一首曲子分两边轮奏感觉像鬼畜

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/9a402dec2e738bd4929fc79aab8b87d6257ff9d0.jpg)

   尝试升级。

   “OS Loader”字样退出历史舞台。

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4e007cd4ad6eddc4fdd1fa5733dbb6fd53663359.jpg)

   ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f3e8e000a18b87d6ce14e2b30d0828381e30fd3a.jpg)

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/fcc53b6134a85edffedbb18f43540923dc547538.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/68c0539a033b5bb5e53d6f523cd3d539b400bcad.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c7b08cf91a4c510ffa97adb66a59252dd62aa5c4.jpg) 两位数表示年份的糟糕设计取消了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e918ed12632762d00804ec13aaec08fa503dc65e.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/25cc6bd6912397dd9cc5d3a85382b2b7d2a287d7.jpg) 水印出现\[冷\]同时banner还加了句广告\[鄙视\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/49d7ba55564e9258a614ce429682d158cdbf4e6b.jpg) 已内置SBPCI128声卡驱动好评。不过显驱没有升级上来。还有，我的VMware Tools呢\[汗\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/dfc99fddd100baa15be00c174d10b912cafc2e47.jpg) 装上显驱。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/9d3036db81cb39db1c90d2fada160924aa18303b.jpg) 服务默认用list方式查看？！一般都是detail来着。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/ef371e300a55b31920aa37d949a98226cdfc17c4.jpg) 啊，看来tools还在，就是不显示图标\[狂汗\]——我更改了一下窗口大小，客户机成功自适应。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/90566bf531adcbef3449caaaa6af2edda2cc9f16.jpg) 这里的图片被线条化了\[弱\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/a00afe24bc315c605048d94387b1cb134b5477b6.jpg) 嗯，稍微伪装一下以后……你会相信这是1989吗\[滑稽\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e17fe0d7277f9e2fab3093a41530e924b999f30f.jpg) 这个选项好评。我已确认在1983没有这个选项。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e4fb2cfafbedab6479a0b26cfd36afc37b311e45.jpg) 合照。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/8f0879168a82b901cd7a3a9f798da9773b12efb9.jpg) cghvbnv22：IE5已经完全完善，喜闻乐见的水印出现。硬盘自检滚动条被砍。 忘了说了，384~390楼是Build1989。 补充一下： Windows 2000 Build 1989 阶段：Beta3 编译日期：1999年2月25日 版本字串：5.0.1989.1 下面是1994。 Windows 2000 Build 1994 阶段：Beta3 编译日期：1999年3月4日 版本字串：5.0.1994.1 继续是散装文件，手动做了个镜像来安装。 升级。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/792fd1fc5266d01657e364849d2bd40737fa359d.jpg) 干嘛在“Windows 2000”之前加个“Microsoft”\[喷\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e71ba91a9d16fdfabf903c42be8f8c5496ee7b97.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/fccad63433fa828b962d784ff71f4134960a5a01.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/13b79cf3b211931355d61a1c6f380cd793238dff.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/327f2011b912c8fc8a621361f6039245d48821fa.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4c07b0cb7bcb0a4631916e956163f6246960afe5.jpg) 哎呀，时间炸弹变严厉了？ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/411d5e00213fb80e8539847b3cd12f2ebb3894ac.jpg) 还真是啊，简直是2K预览版的败类\[吐\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/990db02b6059252d0410f9a83e9b033b5ab5b909.jpg) 改了时间还不行？哦我想起来了，VMware Tools还在幕后自动把时间和主机调齐呢。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3b7df9500fb30f241c8e00afc295d143ac4b037f.jpg) 那只能提前手动破炸弹了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/6050212209f790522cceab9206f3d7ca79cbd5bb.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/0a649102738da97747116a87ba51f8198718e352.jpg) 怎么还…… ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/61cbdf0f7bec54e7c1fef6b2b3389b504ec26a06.jpg) 只能先忍痛割爱了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/39c56d54b319ebc4c45d9a358826cffc1f17166e.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/678bf92e070828388f1930b8b299a9014d08f178.jpg) 过了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e71ba91a9d16fdfaaac12942be8f8c5496ee7be6.jpg) 有点吓人。而且按Enter确认后还会再弹出\[啊\]——NT5怎么又出镜了？……我乱了 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b7f7f68ea0ec08faf21ffb0b53ee3d6d54fbda71.jpg) 太逗比了，问题还没解决，就完成可以重启了\[滑稽\]\[喷\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/86a877395343fbf265f14f8fba7eca8067388fb7.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/61cbdf0f7bec54e7c200f3b2b3389b504dc26aa0.jpg) 显驱成功升上来了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d01b11c7a7efce1b63842266a551f3deb68f65e1.jpg) 第一件做的就是试试修好tools。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3632c0eece1b9d1600744ecdf9deb48f8e5464e5.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b8ede119367adab435f2f1ef81d4b31c8601e476.jpg) 用户文档仍然在%STSTEMROOT%\Profiles ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d17bc7ed08fa513d88f88a73376d55fbb0fbd9c7.jpg) 仍然不太好用的第三方osk。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/678bf92e070828388a0a3db9b299a9014d08f10a.jpg) 它仍然不在Utility Manager ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/6050212209f790522099a79306f3d7ca79cbd58b.jpg) 除了Paint以外的另一个画图软件。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/32fa6bf2d7ca7bcbb7822782b4096b63f424a89c.jpg) 那个外来画图软件的网站还能开\[惊哭\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d17bc7ed08fa513d8d8a8f73376d55fbb3fbd975.jpg) 其他一些小改变：Services等处恢复了details； ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/68cc7831e924b899c2c24d9664061d95087bf693.jpg) 任务管理器多了一个“Show 16-bit tasks”选项。（不好截图） 大Bug：控制面板炸了。 运气好，只是打不开。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/7d9932fab2fb4316ee704bd42aa4462308f7d322.jpg) 运气不好，explorer直接崩溃。 在System32随便翻了翻就找到了来自这些Build的文件： 1378（确实是NT4\[喷\]） 1948 1980（极多） 1982 1983 1984 1985 1988 1990 1992 而1994自己的新文件呢？不到1%。 我们至今找到的所有Build只是冰山一角\[心照不宣\] 合照。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4ab2951ebe096b63789d63fe06338744e9f8ac89.jpg) Windows 2000 Build 1999 阶段：Beta3 编译日期：1999年3月10日 版本字串：5.0.1999.1 兴许是我的BWDB太久没有升级了吧，我的BWDB没有包含这个Build。但是我不得不说它是个“好”Build，因为它有完整的镜像。 既然有个原生可启动的CD，就来一回CD启动的安装吧。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/2ef27a940a7b020873a3604e68d9f2d3562cc828.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/17d876dea9ec8a137370084ffd03918fa1ecc028.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3632c0eece1b9d1689b9c5cef9deb48f8d54641c.jpg)

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e9f52b096e061d950d456b9771f40ad163d9ca17.jpg) 仍然可以把系统安装到FAT（16）分区。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f0a59f188618367a281a217224738bd4b11ce580.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/8b1b11084b36acaf74c8cf5376d98d1000e99c6e.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/327f2011b912c8fc73aeaa62f6039245d7882131.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/36fd2c37acaf2eddf8d91046871001e93801936e.jpg) 插播一句话：建立VMware虚拟机的时候使用1999的镜像，VMware可以识别出是Windows 2000 Professional的镜像！ 噫—— ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/7159acee76094b36f8765f42a9cc7cd98f109daa.jpg) 调时间后。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/ec5b49dca3cc7cd9d85475763301213fb90e911d.jpg)

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/ec5b49dca3cc7cd9da2473763301213fb90e910d.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/c6ec517bdab44aedc352f94bb91c8701a08bfb73.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4f47682542a7d9330fe1a3dca74bd11371f001cd.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/6e29c4cd7cd98d1059dd4b9e2b3fb80e7aec900d.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4903f7539822720e1065a45571cb0a46f01fabef.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/23d305d1f703918faca67a655b3d269758eec41b.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f20f24176d224f4a378634bc03f790529922d173.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/ef371e300a55b3193d80c2da49a98226cefc171d.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3b7df9500fb30f248089acacc295d143ac4b0307.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/4c0056accbef76091b26d83024dda3cc7dd99e61.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3379ce763912b31b53b28e868c18367ad8b4e1bd.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/09a06e22dd54564eee05a696b9de9c82d0584f36.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/36fd2c37acaf2eddf35b0b46871001e93b0193e8.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b8ede119367adab4ad2259ec81d4b31c8501e4a1.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/ab30d04443a9822618bf66888082b9014b90eb1d.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/91b7ca4ad11373f04abf2c30ae0f4bfbf9ed0496.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/89e3183f6709c93de7d94c58953df8dcd000546f.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f2e5f412b07eca8024d87a489b2397dda34483b1.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/16baf559d109b3de1c51a7c7c6bf6c81820a4cac.jpg) 楼上是“CD安装分支”，下面直播一下“DOS安装分支”【误 其实也就是我想看看DOS下的安装界面有没有什么变化。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/6050212209f790528b38089106f3d7ca7acbd56b.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/0bc2cbae2edda3cc3216f78f0be93901233f92a0.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/70ba421e95cad1c8370cb088753e6709cb3d51db.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b32ad38e8c5494ee9bcb43b627f5e0fe9b257ead.jpg) 看来DOS安装界面没有变化。而且在我使用RAMDisk，开了smartdrive还预分配了虚拟磁盘空间的情况下还是极慢\[喷\]DOS下我就不装下去了。 有显驱可装，不亦说乎。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/e71ba91a9d16fdfacbe18841be8f8c5496ee7b81.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/d41a971e3a292df58bfae5bab6315c6035a8735d.jpg) 把玩了一会，目前没找到1999.1什么很特别的地方。明天继续吧。 1999.1没看到什么新功能或变化。我惟一发现的变化是开始菜单\Programs\Startup\下，1994有一个IDW Logging Tools，1999不见了。 拆过炸弹后的合照。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/3b006dd062d9f2d36c7d2a7ea3ec8a136227cc2c.jpg) 刚才奶奶来我家了，我只能陪她说了会话\[狂汗\]下面我们继续 关于控制面板：我发现从NT4升级的1999.1不能打开控制面板，但是从CD全新安装的就可以。想来1994也应该是如此吧。 Windows 2000 Build 2000 阶段：Beta3 编译日期：1999年3月11日 版本字串：5.0.2000.1 跟1999.1一样，2000.1也有完整镜像。而且两个Build是同一天泄露的。那么大概是同一个人放出的吧。 ——2000.1的安装过程，无论是升级还是CD安装都与1999.1毫无二致，略过。 感谢cghvbnv22指点，我找到了资源管理器的全屏功能。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/a9d0df98a9014c0860e37d34007b020879f4f4b8.jpg) 只是有一点比较尴尬![](http://static.tieba.baidu.com/tb/editor/images/client/image_emoticon72.png)

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f3e8e000a18b87d62307ff8e0d0828381d30fdcb.jpg) 这次能找到的新内容就更少了，不过是挨着的Build嘛，情有可原。 硬要挑出来的话，这有一个：回收站的存储目录有了回收站图标。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/b8ede119367adab494beaed181d4b31c8601e428.jpg) 这个呆萌的时钟不知道什么时候出现的，作为独立程序尚未消失。 @12345army ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/f32afb83d158ccbf3a2d23a813d8bc3eb3354180.jpg) 破炸弹后的合照。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/1976d5b6d0a20cf4e6bc214d7c094b36adaf996e.jpg) Windows 2000 Build 2000 阶段：Beta3 编译日期：1999年3月12日 版本字串：5.0.2000.3 Windows 2000测试版中罕见的小版本号不为.1的Build。 安装过程和2000.1基本一样，我不发了。 不过不同的一点是，M$的良心回来了，不再卡到时间不对就不给装下去，而恢复了早期NT5的做法\[真棒\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5185964834/9da0314f9258d109b0b86e20db58ccbf6d814d3a.jpg)

