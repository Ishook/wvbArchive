这个系统最早是上个月发在远景的，现在转过来
（图片是我从远景转过来的，所以带水印）
系统共有8个分卷：
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/d41a971e3a292df57e59a574ab315c6035a8732a.jpg) 
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/dedb600928381f30c88c84c8be014c086f06f02b.jpg) 
***
带有【USB】的分卷集成了USB驱动及两个官方NVMe补丁
USB驱动包含了以下驱动（包括smxdiy论坛大佬修改的版本），适合较新的平台（Intel 300系芯片组、AMD X570芯片组等）安装

> AMD USB3.0 v1.1.0.210
> AMD USB3.1 v1.0.5.3
> AMD USB3.1 v1.0.0.12
> Asmedia v1.16.56.1
> Intel USB3.0 v5.0.4.43
> Intel USB3.1 v5.0.5.55
> Intel Thunderbolt 15.3.39.2
> Nvidia & AMD Type-C

***
带有【无人值守】的分卷内置自动应答文件，自动执行oobe阶段的设置，并以内置的Administrator账户登录系统。
系统源安装盘为MSDN的Windows 7 SP1 64位企业版/旗舰版。使用系统自带的Sysprep工具在审核模式下封装，不包含任何自动激活机制。
补丁更新至2020年2月（KB4539601），系统版本号6.1.7601.24545。所有补丁全部用Dism++固化。
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/e3381bd88d1001e9bbbe1d6eaf0e7bec56e797c2.jpg) 
集成了.Net Framework 4.8及其简体中文语言包及DirectX运行库2010.6月版，未集成VC运行库（一般正版软件安装时都会自动安装所需运行库）。
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/4c23f62297dda144def765d3a5b7d0a20ef486ce.jpg) 
添加了Windows 10的微软雅黑UI字体（msyh.ttc、msyhbd.ttc，msyhl.ttc），以修复IE11部分界面字体显示不正常的BUG。
（IE11新版本的语言包部分界面微软偷懒没有修改字体，仍然会像8.1上的IE11一样调用微软雅黑UI字体，在没有安装这个字体的Win7上会以巨丑的System字体代替显示）
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/e9f52b096e061d952dbe3e596cf40ad160d9cac8.jpg)
使用Win10 1909（PE版本10.0.18362.1，和1903的PE版本相同）的安装程序，以兼容新平台的USB控制器及NVMe硬盘，并支持安装ESD镜像。
修改安装界面及文字为Vista RTM（6.0.6000.16384）的风格。
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/25cc6bd6912397ddd39b91654e82b2b7d2a287e2.jpg) 
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/bb06d5109313b07ea75f59691bd7912395dd8ce2.jpg) 
启动界面默认设置为Vista的滚动条，oobe界面及登录界面改为Vista风格。
（原版Vista登录界面前的徽标动画暂时无解。）
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/0a1949728bd4b31c9ee79dda90d6277f9c2ff8e9.jpg) 
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/a9d0df98a9014c084be021c41d7b020879f4f4e9.jpg) 
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/cae7042662d0f703a5699cbd1ffa513d2497c5e9.jpg)
***
替换默认Aero主题为Windows Vista风格主题，并更改默认Aero主题名称为Windows Aero、Basic主题名称为Windows Vista Basic。删除了除“中国”之外的其它Win7自带主题。
资源管理器底部状态栏高度调整为默认显示三行文字（Vista原版是三行，到了Win7默认变成了两行）。
该Aero主题提取此吧里之前的Win7仿Vista作品【Vista十周年纪念版】。原作者把aero.msstyles里的basic主题改为了vista beta2样式，我又用WindowsStyleBuilder替换回了Vista正式版的basic主题样式。
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/7add4af4e0fe99251cc1603123a85edf8fb171f3.jpg) 
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/1e2beab0cb134954aedbe105414e9258d3094afb.jpg) 
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/cd45ac124954092375ac6a1f8558d109b1de49fb.jpg) 
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/f47beb5594eef01fa6d111a4f7fe9925be317dfb.jpg) 
任务栏默认使用小图标，任务栏按钮设置为“当任务栏占满时合并”，并调节了开始菜单默认显示的项目为Vista的排列方式；开始菜单的电源按钮默认设置为“睡眠”。
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/a00afe24bc315c60965b628e9ab1cb134b5477fe.jpg) 
主题包含最大化熄灯效果，由于win7机制问题，任务栏无法一同熄灯。
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/bdeb2635970a304e990fa89bc6c8a786c8175c93.jpg) 
系统图标替换为Vista样式。（这个截图比较早，左侧“视频、图片、文档、音乐”库图标还是Win7样式，网盘提供的版本里已经替换为Vista样式。左侧字体未改为和Vista原版一样的蓝色）
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/83099b029245d688001abac5b3c27d1ed31b24a8.jpg) 
替换Windows侧边栏为Vista版本，原版的股票、天气组件已经停止服务，找了两个第三方制作、界面相似的替代。删除了右键单击桌面的“小工具”菜单。
（由于Win7机制问题，在按Win+D或单击显示桌面按钮时，边栏小工具会一并隐藏）
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/3304e5035aafa40fbcc0c6bcbc64034f79f01946.jpg)
***
8个分卷中有4个名称中带“X”的版本，除了具备上述所有特点之外，还做了以下额外的修改：
系统设置默认禁止程序锁定到任务栏。（可以通过组策略重新开启：用户配置——管理模版——“开始”菜单和任务栏，在右侧打开“不允许将程序附加到任务栏”，选择“已禁用”确定。）
替换部分系统附件程序（DVD Maker、画图、计算器、写字板、Windows 联系人）为Vista版本。
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/4aa1d418ebc4b7454036bf77d8fc1e178b821521.jpg) 
提取Vista自带的Windows Media Player 11替换掉Win7的Windows Media Player 12。
保留原版的首次使用设置向导，Windows Media Player工具栏工作正常，双击文件打开WMP工作正常。
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/b828b601baa1cd11b9297a41ae12c8fcc2ce2d2d.jpg) 
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/94cbe095a4c27d1e0ab933a50cd5ad6edcc4382d.jpg) 
添加Vista中的Windows日历、Windows Mail等Win7不自带的程序。（Windows日记本未移植）
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/8be72e550923dd54fefdaf09c609b3de9d82483e.jpg)
***
6楼被吞了，重发图
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/dba428c3d5628535681bda4087ef76c6a5ef63c9.jpg) 
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/8eeffa17fdfaaf51651889de9b5494eef21f7ac9.jpg) 
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/3632c0eece1b9d16693c9200e4deb48f8e5464c9.jpg) 
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/b32ad38e8c5494ee6ad907783af5e0fe9b257ec9.jpg) 
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6539461691/3b1833e636d12f2e31fea60158c2d562873568c9.jpg)
/s/13iN75-8px01BR4UtGOIbOA 密码：pudp
***
使用说明：
直接将ISO写入U盘安装即可，如果在新平台下安装，需和Win7一样在BIOS中启用CSM支持。也可在PE下手动安装镜像sources目录下的install.esd文件。
镜像中内置了一些“可选安装包”，位于根目录Optional Package目录下，分别为：

> Classic Shell 及皮肤——更精致模仿Vista开始菜单，也可使用在Win7中被移除的经典开始菜单
> Windows 7 Build 6801 启动画面——替换启动画面
> Windows Live 照片库——用于在Win7下体验Vista版 “Windows 照片库” 的替代方案
> 第三方软件添加网络图标闪烁动画——在Win7上实现Vista的“启用网络动画”功能，在网络有数据传输时会闪烁
> 第三方软件给图标添加排序功能
> 修改系统Service Pack版本号为SP2
> 这些工具可以帮助实现一些在Win7上被移除的功能，达到更接近Vista的体验效果。
> 每个目录下都有简单的说明文档，可自行查看。

***
部分问题解答（相比远景原帖删除了几个过于小白的问题）：
Q：既然要更好地兼容新硬件，为何不基于Win10或Win8.1等更新的系统修改？
A：主要有以下两个原因：
（1）Win8.1开始，微软给部分系统核心dll添加了数字签名及验证机制，对它们进行修改会破坏签名，导致无法进入系统。
（2）Win8.1和Win10都不带Aero，需要使用第三方付费软件Aero Glass还原Aero效果，而该工具难以封装到系统中。
***
Q：这个系统可以用BypassESU破解然后打ESU补丁吗？
A：可以，但最好使用非X版，这是由于BypassESU破解工具中包含的微软KB4528069补丁会替换Vista版计算器为Win7原版，造成计算器无法使用。如果要在X版上使用BypassESU，请提取原版Windows 7 64位的C:\Windows\System32\zh-CN\calc.exe.mui，在PE下覆盖本系统下相同位置的文件。
因为一部分修改通过修改系统DLL资源来实现，而后续的ESU补丁有可能会把这些文件升级回Win7原版，造成修改效果丢失，所以打补丁之前要谨慎，最好对整个系统做一份备份。
***
Q：为什么要把历史补丁全部固化不允许卸载？
A：系统采取替换部分系统文件资源的方法来实现精仿Vista，而补丁在安装时都会把被替换文件的当前版本在winsxs文件夹里额外存放一份，作为卸载更新时的后备资源。Win7发布至今，某些文件已经被替换过了N多个版本，它们版本号不同不可互相通用，对涉及到文件的每个版本都进行修改工程量太大，时间上精力上作者个人都无法实现。同时，因为同样的原因，这个系统不能运行sfc \/scannow命令进行系统文件的修复。
***
Q：这个系统可以二次封装吗？
A：非X版可以，但因为部分功能的实现依赖个人编写好的自动应答文件和脚本，直接封装再部署可能会造成部分功能特征消失。X版不可以，因为配置WMP的过程涉及修改大量注册表，经作者实测封装后再次部署会中途出现错误，导致安装无法完成。
***
Q：用Office Tool Plus工具安装新版Office失败，提示建议更新到Windows 10？
A：Office 2019和Office 365从2020年3月的版本开始不再支持Windows 7系统，请安装2002或更早的版本。
***
Q：这个系统仿得并不像，很多细节都和Vista有差别，我还不如直接用原版的Vista。
A：Windows 7毕竟在Vista的基础上进行了部分功能项和系统API的调整，而Windows是闭源操作系统，因此一些因为机制原因无法做到仿Vista的细节基本没有好的解决方法，或是依赖第三方软件，或是彻底无解。虽然通过简单替换Vista版DLL的方法可以移植部分Vista界面和系统功能到Win7中，但大多都不完美，一些功能无法使用。
个人制作这个系统的目是在较新的机器上实体安装来获取Vista的体验（因为Vista对新硬件新软件都缺乏良好支持），所以经验证不完美、影响功能使用的修改方案我个人大多不会采用。如果只是想偶尔尝个鲜，并不打算长期使用Vista风格的UI，建议使用虚拟机体验原版Vista。
***
待改善的地方：
> 手工建立的快速启动栏在封装部署之后会消失
> 部分系统文本未替换成Vista中的叙述（如“入门”——“欢迎中心”、“操作中心”——“安全中心”）
***
又被吞楼了，或许是含油管地址的原因……
***
再次感谢以上作者修改的vista主题：
@lsqsjz 