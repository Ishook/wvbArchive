# 不得不说，TweakNT是个破

不得不说，TweakNT是个破解NT6以下系统时间炸弹的神器。但是像NT5 Beta这种地方，可能会运行不了TweakNT。我正在试图找到TweakNT的工作原理，以便有时有需要可以手动破炸弹。 有人猜想过TweakNT是通过修改Winlogon破解炸弹的。可是我发现我用TweakNT破了炸弹的Longhorn的Winlogon并没有被修改过的痕迹（文件修改日期还是版本编译日期）。抱着疑惑，我拿一个专门监视文件操作的软件看了TweakNT运行时发生的文件操作，发现只动了SOFTWARE文件。晕，SOFTWARE不就是注册表吗\[狂汗\]所以还是要从注册表下手。 先开一个TweakNT ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/0a1949728bd4b31c8465fe1a8dd6277f9f2ff82f.jpg) 再开一个RegFromApp ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/27fdae3c70cf3bc72ee0a74ddb00baa1cf112aa0.jpg) 胡乱加个炸弹【 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/f1c154fb828ba61e09659d8e4b34970a324e59f9.jpg) 好了，记一下这些注册表操作。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/7b33f83cf8dcd100093ead80788b4710bb122fe2.jpg) 右下角的水印什么鬼了啦233不过这不是我们关注它的时候。现在去炸弹。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/d41a971e3a292df5664df8b4b6315c6036a873fe.jpg) 这个应该更关键。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/8a7402390cd79123ce64c0d5a7345982b0b78084.jpg) 炸弹时长11天： ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/bcf7f544d688d43f3f89c353771ed21b0ff43b60.jpg) 1天呢？ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/c760c3c37d1ed21bb56d7344a76eddc453da3fe4.jpg) 再多做了几次试验，`PriorityQuantumMatrix`各个键值： 去炸弹：`70,95,FE,1F,00,00,00,00,08,DD,D1,01` 1天：`70,95,FE,1F,A0,05,00,00,08,DD,D1,01` 2天：`70,95,FE,1F,40,0B,00,00,08,DD,D1,01` 3天：`70,95,FE,1F,E0,10,00,00,08,DD,D1,01` 4天：`70,95,FE,1F,80,16,00,00,08,DD,D1,01` 5天：`70,95,FE,1F,20,1C,00,00,08,DD,D1,01` 这个规律看上去并不显明。 10天：`70,95,FE,1F,40,38,00,00,08,DD,D1,01` 21天：`70,95,FE,1F,20,76,00,00,08,DD,D1,01` 43天：`70,95,FE,1F,E0,F1,00,00,08,DD,D1,01` 63天：`70,95,FE,1F,60,62,01,00,08,DD,D1,01` 99天：`70,95,FE,1F,E0,2C,02,00,08,DD,D1,01` 100天：`70,95,FE,1F,80,32,02,00,08,DD,D1,01` 274天：`70,95,FE,1F,40,05,06,00,08,DD,D1,01` 677天：`70,95,FE,1F,20,E0,0E,00,08,DD,D1,01` 动的只是其中的24个bit。 目前没研究出什么，只知道： 1.只要Timebomb期限不要长到TweakNT受不了的程度，`PriorityQuantumMatrix`的值就只有左起第5、6、7byte是变化的。 2.在期限变化不大的情况下（如677天与678天、679天的值相比），第7个byte也不会变化。这么说我怀疑是不是加密的时候把高、低位打乱过。 规律找出来了！ 各位要是有兴趣就试试看自己找一找，明天我公布。 好了，现在我讲讲如何解码那段注册表。 前面如图所示的`HKEY_LOCAL_MACHINE\TWEAKNT\ControlSet001\Control\Session Manager\Executive\PriorityQuantumMatrix`（实际位置是`HKEY_LOCAL_MACHINE\SYSTEM\ControlSet001\Control\Session Manager\Executive\PriorityQuantumMatrix`），目前已经确定第5、6、7byte与炸弹长度有关。其他部分尚不明确与什么有关，到我装的其他虚拟机就不一样了，但是应该不会影响我们破解炸弹了吧。 第5、6、7byte与日期的关系如下：（以下数字全部是16进制下的） 首先，将时间炸弹的天数乘上`5A`。例如，`6E9`天的炸弹，先要乘上`5A`，变成`26DEA`。 然后，按需在左边补上0，凑成6位的数。例如，`26DEA`补成`026DEA`。 最后，直接调换各个数位的位置。如下： （最高位）（第2位）（第3位）（第4位）（第5位）（最低位） 变成： （原最低位）（原最高位）（原第4位）（原第5位）（原第2位）（原第3位） 例如，`026DEA`变成`A0DE26`。 变换后得到的数字即是TweakNT会写进`PriorityQuantumMatrix`第5、6、7byte的值。 例如，原来注册表的`PriorityQuantumMatrix`如果是 `70,95,FE,1F,00,00,00,00,08,DD,D1,01` 加上`6E9`天的炸弹后就成了： `70,95,FE,1F,A0,DE,26,00,08,DD,D1,01` 如果没有炸弹，那么数值计算就取炸弹天数为0。至于炸弹0-day好像并不存在——我记得Longhorn 3790也就是0-day激活而不是0-day炸弹吧。 至于`HKEY_LOCAL_MACHINE\TWEAKNT\Setup\SystemPrefix`（实际为`HKEY_LOCAL_MACHINE\SYSTEM\Setup\SystemPrefix`）也是类似的加密。 只不过，与时间炸弹相关的byte是第3、4、5字节；要乘上的数是B4；补足6位数后，这样调换数位： （最高位）（第2位）（第3位）（第4位）（第5位）（最低位） 换成： （第5位）（最低位）（第3位）（第4位）（最高位）（第2位） @微軟藍澤光

我楼上讲那些也只是纸上谈兵。刚才在2072上实践了一下，获得成功。在破炸弹之前winver会显示一个expire日期，现在没了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/833aa4fcfc03924529facaac8d94a4c27c1e253f.jpg) 目前还有最后一个问题要解决： 动`HKEY_LOCAL_MACHINE\SYSTEM\ControlSet002\Control\Session Manager\Executive\PriorityQuantumMatrix`的时候，没有任何困难。但是动`HKEY_LOCAL_MACHINE\SYSTEM\ControlSet001\Control\Session Manager\Executive\PriorityQuantumMatrix`和`HKEY_LOCAL_MACHINE\SYSTEM\Setup\SystemPrefix`的时候，每改完一个，刷新一下就恢复到没改时的值。我认为可能有线程在保护这两个值。目前我采用的办法是启动PE，在PE里挂载SYSTEM文件然后更改——也就是到Beta系统外去更改。这个办法忒笨了，我在想能不能像TweakNT一样在Beta系统内解决。 安全模式是不行的。 又试了试将注册表设置权限。即使只给系统以读权限而不给系统以修改权限，系统照样能改回去；如果什么权限也不给系统，那么启动时会蓝屏。 好吧，还是PE修改比较好用。将破炸弹过程总结成小白都能看懂的教程： 1.在安装了Windows NT5/2K测试版的机器（当然平常都是虚拟机）上启动一个Windows PE，打开regedit。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/2ef27a940a7b020846483f4568d9f2d3552cc882.jpg) 2.选中`HKEY_LOCAL_MACHINE`，点击文件-&gt;加载配置单元。定位到 测试版系统目录（一般是`C:\Winnt`）`\System32\config\` 目录下。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/4e007cd4ad6eddc4a378b45f33dbb6fd506633e8.jpg) 3.打开SYSTEM。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/f08aad8165380cd71547a249ab44ad345882812a.jpg) 4.起个名字挂进去。就跟着我起名sys好了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/0a1949728bd4b31caabd941f8dd6277f9c2ff882.jpg) 5.挂载后，点进`HKEY_LOCAL_MACHINE\sys\ControlSet001\Control\Session Manager\Executive\`。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/edc03e83b2b7d0a287900439c1ef76094a369a2a.jpg) 6.双击开始修改`PriorityQuantumMatrix`的值。将如图的这一段数据（第5、6、7byte） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/dfc99fddd100baa111684a1f4d10b912cafc2ec7.jpg) 换成`000000`。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/411d5e00213fb80ee2af61733cd12f2eb8389409.jpg) 7.点进`HKEY_LOCAL_MACHINE\sys\setup\`。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/f3efd750f819861811d9ef2040ed2e7389d4e6e9.jpg) 8.双击开始修改如图这段数据（第3、4、5byte） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/a9a4522bc65c10382fffce66b8119313b27e8982.jpg) 也改成`000000`。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/8c4b0b80800a19d87b5a84a139fa828ba71e462a.jpg) 9.点中sys， ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/32fa6bf2d7ca7bcb50f9ca8bb4096b63f424a88d.jpg) 点击文件-&gt;卸载配置单元。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/cde466e83901213f2c0142785ee736d12e2e955d.jpg) 10.重启。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/750e81cc7b899e51f39a36b048a7d933c9950d77.jpg) 11.进入你的NT5/2K 系统。打开winver，不再显示Expire日期了。Enjoy it！ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/a00afe24bc315c6085bc644b87b1cb134854775a.jpg) 与未破炸弹的进行对比。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5197847676/967cb33e8794a4c29a58e88f04f41bd5ac6e3914.jpg)
