1L祭天
首先，BUG10兼容性差到了极点，一些旧版复刻组件是绝笔不能复刻成功了这次发布的主要是游戏+一些勉强复刻成功的组件包含：WMCw7游戏墨球（显光标）三维弹球Tinker （这个有彩蛋，居然关于里显示的是vista UltimateHoldEM 这个貌似国内的Ultimate Extras没有毕竟是XXXX在线发牌游戏Live软件包2009全家桶可自选
究极版hosts1.本hosts基于Github的googlehosts和gfwlist两个项目为基础加上一些本人自收集的网站集合而成2.不要期望着hosts支持所有网站，实际上这个hosts只支持被DNS污染以及HTTP被RST但HTTPS正常的网站至于Google的大部分服务、Facebook、Twitter以及一众被SNI RST的网站还是趁早打消念头去找软件吧3.希望在使用hosts的同时不要做出违反当局的行为4.时间不够一堆网站可以到gfwlist里慢慢找、慢慢加（PS:gfwlist是BASE64编码，反编译就OK了）https://raw.githubusercontent.com/gfwlist/gfwlist/master/gfwlist.txt
https://pan.baidu.com/s/1WmbiL7AP_ZEz1mvm7ydr9w
组件正在上传中hosts用法：直接丢到%SystemRoot%\System32\drivers\etc就OK了PS:BUG10可能会提示权限不够，这个时候请右键hosts文件属性-------安全--------编辑——将ALL APPLICATION PACKAGES的完全控制勾上（确保自己是管理员）复刻组件用法上传完后一一介绍
复刻包的正确安装步骤：1.安装w7游戏（Win7Games4Win10_8_81_v2）解压完之后一路下一步就OK了效果图（win10 1803备用机实体机测试）
补图
2.安装Tinker、HoldemTinker解压到之前的安装目录即可Holdem解压后运行Install.bat即可（位置任意）PS:Tinker的关卡编辑器和HoldEM只有英文（Tinker的关卡编辑器有简中但中文网站没有，MS官网链接撤了）效果图：
3.三维弹球、墨球（Pinball和Inkball）复制到之前游戏的安装目录即可效果图：细心的人可能会发现下面的两个彩蛋
![](3.WMC具体参考http://tieba.baidu.com/p)
![](其实我觉得最难攻关的三关就是这三关：1.游戏其实难度最大的就是w7游戏，毕竟改的费神的多，后来还是借用的http://www.winaero.com的老外作品，还是感谢了。最棘手的是Tinker，主要还是难在验证部分，w7实测直接vista兼容性ok，但bug10水土不服啊，直接提示软件只能在vista ultimate运行，后来翻游戏破解方面的资料的时候偶然想到NOP指令（16进制下找出验证部分并改为0x90，毕竟是离线游戏又不和游戏平台沾边当然容易一点）成功解决验证。最难找的是墨球和Holdem，后来我花了5毛远景代下（原版容易提取，但修改版难找，用不知道怎么修改）+google)
Ver1.1更新日志:
1.添加挖耳街 wsj 曰报和锝国之生 dw以及一些下载apk的网站
2.修复亚马逊AWS，避免部分地区丢包导致的无法访问
2.去除非死不可的大部分hosts指向，减
小体积（已查明这批ip已经进入黑名单）
*.未来考虑更新日志使用CPY破解组的信息发布方式。（SNI RST貌似在深夜不断刷新就有几率避免RST）
4.尝试修复部分google服务
预计近一两天发布
***