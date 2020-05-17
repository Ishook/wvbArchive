# 【某尚未想好标题的专栏】（一）vista 64bit的配置

最近考完试了，实在是挺无聊的，那就写些东西吧 本专栏的内容其实我还没想好来着，但大体上主要是想把一些很难搞的问题或者有很多坑的地方汇总一下，以方便之后有需要的人看和避免踩坑，欢迎各位提一些建议 而先写vista 64bit的配置主要因为本吧的名称也含有“vista”，而且64bit的vista如果要基本当成win7 64bit用实在是太多问题了\[狂汗\]（但是32bit的却好的多得多），这些问题要解决都并非容易，，不过通过我334天的努力，已经解决掉了一部分\[滑稽\]（至少我现在用起来已经没有什么问题了），因此写个东西出来方便如今还想用64bit的吧友看看。

PS1:本系列文章将不会过多介绍驱动、硬件之类的问题，一来是我的电脑是11年买的，目前用了那么多年来就没有遇到过任何的硬件/驱动问题，因此没有过多研究，二来是因为我对硬件/驱动等并不是非常了解，因此就不怎么在这里介绍\[滑稽\] PS2:版权问题：除了我特意说明外，随意转载

显卡驱动之坑一：关于intel集显 intel集显不建议在官网下载驱动，而建议在windows-管理中用设备管理器安装驱动，如果你在官网下载安装intel集显驱动，在玩某些RPG，推黄油（划掉\[滑稽\]）Galgame，和玩某些上古dos游戏的时候，当你全屏的时候，会发现游戏界面并没有被按比例放大，而是旁边多出了一大块黑边，用windows画图画出来就像是这样 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6011537653/2b9791256b600c33ab2c8135174c510fdbf9a1ef.jpg)

蓝牙驱动之坑二：如果你购买了外置usb蓝牙，最好不要安装厂商内置的驱动，而是使用windows设备管理器来安装，如果你使用的是厂商的驱动，对vista兼容并不好，也就是说你在重新启动计算机之后怎么都无法连接上蓝牙\[喷\] 但是使用windows默认驱动的话，又有一个坑，你连接蓝牙之后音质很垃圾，原因是vista对蓝牙耳机/音响默认使用的是双工电话这个音质，你需要改一下设置 第一步，打开控制面板，找到蓝牙管理器 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6011537653/eb90644e78f0f73676e412fc0755b319eac4132e.jpg)

双击进入，找到你的蓝牙耳机、蓝牙音箱，右键 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6011537653/4ab2951ebe096b63de5d00ad01338744e9f8acf8.jpg)

找到服务选项栏，取消标记“免提电话服务“，标记”耳机”，“音频接收器” ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6011537653/e0186ffb513d26974d3456a058fbb2fb4116d859.jpg)

回到控制面板，选择声音 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6011537653/27fdae3c70cf3bc73e239411dc00baa1cc112a25.jpg) 然后右键你的设备，选择“设置为默认设备”

二.关于续命补丁 不建议安装，主要原因是续命补丁会造成许许多多的问题，比方说2018年3月的续命补丁对于某些电脑来说会造成注销用户蓝屏的问题，因此如果实在非常在意安装补丁的话，请使用windows server 2008

三.关于输入法在cmd中的输入问题 vista中的输入法配置算是最奇葩的一个了...当时我折腾在cmd中输入中文搞了半天\[狂汗\] 解决方案：先安装好你喜欢的输入法，然后打开控制面板，找到“时钟，语言和区域” ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6011537653/65d9b32b2834349b37a93678c4ea15ce34d3be91.jpg)

打开区域和语言选项 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6011537653/3fca0008c93d70cfa400f2f0f5dcd100b8a12b4e.jpg)

找到“键盘和语言”，单机“更改键盘” ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6011537653/0fbe47a5462309f78ca1f5ef7f0e0cf3d5cad672.jpg)

在“默认输入语言”这一栏中务必使用你选择的中文输入法 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6011537653/43cf3cb4c9ea15ce0186bbf4bb003af33887b2dc.jpg)

在底下我框着的这一栏中务必把你选择的中文输入法放在第一位，并且删除原来的貌似叫做中文-英语还是中文-拼音什么鬼东西的（忘记了...）然后在底下点右边的天价，选择英语（加拿大）（如果不这样做的话，会导致到时候cmd中无法输入""@"

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6011537653/3632c0eece1b9d1691ebc09cfedeb48f8d546410.jpg)

然后关于在cmd中切换输入法的问题：cmd中只能使用shift+alt切换输入法，其他快捷键都无效。

首先，极其不建议在9102年在生产力计算机上使用vista 64bit，主要原因是你可能随时会遇到许许多多奇奇怪怪的问题。 一.安装阶段 请不要使用PE安装，主要原因是vista封装时候的一些问题，如果你使用PE安装，会导致你的vista安装的盘符是D：虽然看上去没啥问题，但是在安装某些软件的时候就会出现一些问题了，比如无法安装，安装后无法打开（提示什么什么配置错误等等），并且别妄想安装完之后用diskgenius之类的软件更改盘符，的确，这可以被更改，但是更改完之后你会发现你的桌面壁纸变黑，并且几乎所有软件无法运行。 第二，请最好使用打满补丁的（主意：尽量不要选择打了续命补丁的！！参见二）vista，这样可以节约你打补丁的时间 四：在64bit的vista上使用安卓模拟器 这是一个非常非常非常\*\*的问题\[黑线\]，貌似是因为vista重组之后使用win server 2k3的原因，导致了市面上90%的安卓模拟器无法正常运行 警告：谨慎安装待会我提到之外的安卓模拟器，因为有的安卓模拟器安装之后会导致你的用户PATH炸掉，具体情况是，chrome下载完文件后点击“在文件夹中打开”无效，对快捷方式右键点击“打开文件位置”无效，对于这个问题其实是有解决办法的，那就是把你的用户删除，新建一个用户即可，当然了，如果你非得测试一些安卓模拟器，也建议你新建一个用户来测试

列举一些我安装过的安卓模拟器兼容情况 夜神安卓模拟器：新版本可以安装，无法运行。旧版本安装后会导致PATH错误！！ 蓝叠安卓模拟器：可以安装运行，什么问题，缺陷是无法使用虚拟摄像头，导致你无法扫描二维码

网易MuMu助手：可以安装运行一次，会导致PATH错误！！ 逍遥安卓模拟器：可以安装运行，但是打开的时候有几率会出现打开到40%左右闪退 雷电手游助手：无法运行 小皮助手：可以运行，但是在里面使用麦克风会出现音质很差的问题，并且这个安卓模拟器兼容性不太好，而且安卓模拟器的包无法被安装到C盘，他会自己选择空间最大的一个盘安装 天天安卓模拟器：无法运行 小蚁安卓模拟器：可以运行，兼容性还可以，但是有一个致命bug，切换用户的时候会导致安卓模拟器崩溃！！ 叶子猪安卓模拟器：可以运行，但是无法模拟定位，而且we&ch（at）运行卡顿 靠谱助手：无法运行 其他的暂时想不太起来了，但是我就记得当时花了好几天把市面上几乎所有安卓模拟器都试了一遍

在安卓模拟器上有一个无法解决的bug：有的安卓模拟器使用新版的virtualbox，这会导致注销的时候安卓模拟器崩溃。 五：浏览器问题 这是一个重头戏\[狂汗\]因为各大浏览器甚至在vista还没有停止技术支持以前就先不支持vista了，这导致了使用各大浏览器浏览现在的网页存在许多问题 这里我不得不承认，如果你不是很在意fq信息泄露，或者你本来就习惯了使用国产浏览器，那就是用国产浏览器好了，当然，如果你坚持使用IE，FF，chrome也是可以的，待会接着讲怎么样让IE，Chrome，FF在vista上体验变好。

先从IE说起 由于vista不支持tls1.1/1.2，因此IE很多页面都无法打开，这个时候就需要安装一下tls1.1/1.2 的支持 下载该补丁 [https://www.catalog.update.microsoft.com/search.aspx?q=4056564](https://www.catalog.update.microsoft.com/search.aspx?q=4056564) 然后双击安装（如果无法安装请使用dism++安装） 然后下载这个reg [https://johnhaller.com/sites/default/files/downloads/reg/vista-tls-1.1-1.2-update.reg](https://johnhaller.com/sites/default/files/downloads/reg/vista-tls-1.1-1.2-update.reg) 导入，重启电脑 然后在控制面板找到Internet选项（如果在IE中打开会找不到开启tls1.1/1.2的选项） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6011537653/49d7ba55564e9258ace2c7139182d158cebf4e6a.jpg)

切换到“高级” ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6011537653/c7f5c68a87d6277f705172c525381f30eb24fc86.jpg)

然后找到这里，如果你安装了这个补丁的话（我这里没有安装）会出现使用TLS1.1和使用TLS1.2两个选项，把它打钩，重启电脑，即可 当然这样做还不够，因为很多网站根据user-agent来判断的，所以就算你开启了使用tls1.1/1.2也没用，你还得要修改user-agent（具体就请自己百度了，因为第一百度有很多这样的资料，第二我自己不用IE，所以也不是很清楚），修改user-agent的原则是优先换版本（即把IE版本提高）如果不行换系统（即把系统伪装成win7或者win10，当然我建议伪装成win7，因为伪装成win10可能有的网站会让你使用edge= = ）如果还不行的话才建议换浏览器（比如伪装成chrome60,70这样） 至于如何获取别的浏览器的user-agent，请使用goog（le），在其中搜索你想要更换的浏览器user-agnet+系统，比方说输入windows7 IE11 user-agent选择第一项一般就能出来这样的结果了，这就是user-agent了 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6011537653/4aa1d418ebc4b745974ff4ebc2fc1e178882156d.jpg)

好的让我们说说FF，FF的话建议使用ff52 esr，然后其他的话....好像没啥好说的了，因为我也不用ff，当然ff52有个很烦的问题，那就是总是会蜜汁卡顿，如果你对防查水表有很高的要求的话请不要使用ff。 当然了，ff52对html5支持也不好，导致播放html5视频卡卡的 PS：ff可能出现h5视频无法播放，解决方法：[http://mozilla.com.cn/thread-385112-1-1.html](http://mozilla.com.cn/thread-385112-1-1.html)

本楼因为蜜汁原因被识别为涩擎，因此只好发图片\[黑线\] ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6011537653/b6d00c610c338744f15c67815c0fd9f9d52aa0a3.jpg)

六：Vmware问题 vmware虽然官方说是vm10是最后一个支持vista的版本，但是实际上绿色版的vmware12.0是最后一个支持vista的vmware版本，但是实际上这有一个很大的bug，那就是usb无法被连接到虚拟机内，提示要安装什么驱动，但是安装会失败。 所以，请不要使用绿色版的vmware12.0，如果你一不小心安装了，解决的办法是运行安装目录下的卸载.bat，然后重启电脑，删除所有注册表内关于vmware的项目，再次重启，安装安装版的vmware10即可 虽然绿色版的vmware11目前看来没有什么大问题，但是不建议使用。vmware11对于vm10也没有改进太多，而且万一有bug出现你也很难定位是vmware的问题

七：Vocaloid问题 进测试，vocaloid5，vocaloid4的最新版（v4的老版本例如4.0x版本我没试过，懒得试了= = ）不过vocaloid3可以使用，目前看来有一个无法解决的bug，那就是让虚拟歌手发前几个音的时候会感觉卡卡的，断断续续的，这是bug来的，当你导出到wav就会发现播放的很流畅，所以请各位调音师不要在这里纠结了...任凭你如何调颤音，十大参数都没用的

八：开机在桌面任意位置右键卡死或者卡很久 这是软碟通的问题，请升级到最新版。

九：cmd中切换到中文输入法按win+d显示桌面后再用鼠标点击有几率系统死机 这是由于你使用了第三方修改的vista的问题，所以请在cmd中使用sfc /scannow进行修复即可

十：系统开机硬盘占用高 主要有两个原因 1.你使用了逍遥安卓模拟器等开机启动的安卓模拟器 2.你使用了国产（这里特指电脑管家，360卫士等）安全防护软件，它们对vista支持不好导致的

十一：杀毒软件 不建议使用国产杀毒软件，兼容性差会导致系统卡顿，建议使用自带的windows defender（病毒库手动更新在[https://www.microsoft.com/en-us/wdsi/definitions）](https://www.microsoft.com/en-us/wdsi/definitions）) 如果非得用第三方杀软，建议用轻量级杀软

十二：Git的使用 最新版本的git不支持vista，请使用2.13版本（太老无法正常使用） 给个链接：[https://tpedutw-my.sharepoint.com/:u:/g/personal/redapple0204\_tp\_edu\_tw/EbGd8\_nz8oVAgzWH3WBr-qYBkqaKmXvB48PzQlHIfHMd0g?e=acdITU](https://tpedutw-my.sharepoint.com/:u:/g/personal/redapple0204_tp_edu_tw/EbGd8_nz8oVAgzWH3WBr-qYBkqaKmXvB48PzQlHIfHMd0g?e=acdITU) 关于汉化： 教程：blog.csdn.net/woshiniudun/article/details/58231044 涉及到的文件：[https://tpedutw-my.sharepoint.com/:u:/g/personal/redapple0204\_tp\_edu\_tw/EUX\_wGrp0zdLo004GFQD0j0BtrZRGffYQap-DlYiag4vgA?e=EIVzxf](https://tpedutw-my.sharepoint.com/:u:/g/personal/redapple0204_tp_edu_tw/EUX_wGrp0zdLo004GFQD0j0BtrZRGffYQap-DlYiag4vgA?e=EIVzxf)

十三：关于Galgame 由于vista游戏渲染的问题，能在vista上运行的Galgame会比RPG和上古dos游戏出更多的bug，比方说到目前为止我试过的所有galgame在玩的时候除非按游戏内的退出，否者按win+d都无法返回桌面！！（查水表警告） 而且请不要在游戏过程中按win键，要不然你的屏幕分辨率会变成这个鬼样子 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6011537653/bcf7f544d688d43f7f17800d701ed21b0cf43b8c.jpg)

而且这个时候如果你游戏下面还开了别的窗口的话，会导致游戏下面的窗口错位，大小不正常等等问题，所以在运行游戏之前最好不要留窗口在底下.

十四：关于trim vista下可以使用第三方工具进行trim，比方说之前我有ssd的时候就用的是O&O Defrag Pro，请下载最新版并且在设置里设置6小时trim一次，经过我的测试这款软件是真的能够trim的 至于别的例如ADATA SSD ToolBox等工具，反正进过我的测试它内置的trim在vista上不起作用。 PS:请不要使用TrimSSD这款工具，这款工具在我这里测试会导致整个ssd数据被完全清空，可能是bug来的（毕竟个人写的） PS2：trim是否成功检测工具[https://github.com/CyberShadow/trimcheck](https://github.com/CyberShadow/trimcheck) 使用方法：trim之前运行一下这个程序，trim之后在运行一次，看这个软件返回过来的信息就知道是否trim成功 注意：最好多测试几遍，可能一次不准

十五：安装完毕硬盘空间占用太大 vista和win7都一样，会默认在c盘创建一个和你RAM一样大小的虚拟内存文件，所以在设置里改下就好

番外：vista最后支持的软件列表

