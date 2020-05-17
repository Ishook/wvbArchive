上次老v吧发的那个比较水，那么重新整理发布一下
Vista与win8+的系统启动管理器是不能共存的，否则vista会蓝屏
所以这个帖子旨在解决这个问题
看此贴之前，建议弄懂以下几个概念
1.UEFI引导与传统引导的区别
2.ESP（EFI启动分区）
3.Bootmgr（Windows启动管理器）
4.BIOS
5.双系统
6.分区
首先我们需要一个UEFI启动的win8/10
在磁盘管理中，我们可以看到:
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/7627b238b6003af3dab624df3c2ac65c1138b673.jpg)
如果你的uefi下的win8/10是比较默认的分区布局，那么就会如此：
第一个标有恢复/recovery的是恢复分区
第二个是EFI系统启动分区
第三个在磁盘管理中隐藏，但是通过其他软件或diskpart可以看到，是msr保留分区
第四个就是系统盘
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/891e72cf36d3d5396b5bf47c3387e950342ab025.jpg)
确认好并对应好每个分区之后，我们继续
1.准备好安装vista的分区
2.准备好vista镜像（必须x64至少sp1）
3.确保开启主板BIOS里的CSM兼容模式
4.确保关闭主板BIOS里的Secure Boot安全启动
5.建议主板BIOS里调整为UEFI only/仅UEFI启动
6.准备好支持UEFI启动的winpe（推荐win8/10pe x64）
重启，从uefi winpe启动电脑，然后启动diskpart
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/f32afb83d158ccbf498b558510d8bc3eb035414b.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/4903f7539822720eb7f5024572cb0a46f31fab48.jpg)
选择你的磁盘（efi分区所在的）
几个需要用到的diskpart命令/名称
sel - 选择
disk - 磁盘
part - 分区
vol - 卷
ass - 分配盘符
list - 列出
exit - 退出
***
比如我要查看有哪些磁盘，输入：
list disk
我要选中磁盘0：
sel disk 0
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/16baf559d109b3debd2407d7c5bf6c81820a4cef.jpg)
接下来，列出这个选中的磁盘（disk）包含的分区（part）
先列出分区：
list part
我们看出，此例中，分区2标明“系统”，容量也与之前磁盘管理中看到的EFI分区吻合，那么这就是EFI分区了，我们把它选中
sel part 2
然后输入ass给这个默认隐藏的efi分区分配盘符，使我们得以访问
#注意，EFI分区需要system/Administrator权限才能访问，所以我在PE下操作
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/ed9abac551da81cb6b746e725b66d0160b2431f0.jpg)
我们打开刚分配盘符的EFI分区，看到一个EFI文件夹，把它复制走，之后将会多次需要它
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/c27fc11fa8d3fd1f6af34e85394e251f97ca5f88.jpg)
***
然后重启回到系统中
接下来，就像UEFI装win7一样，我们要给vista镜像加入Bootmgfw.efi，然而与装win7不同的是，由于vista与win8/10的bootmgr不兼容，不能像win7一样直接提取win8/10的bootmgfw，而是要从另一台已经安装好的uefi win7/vista上提取，这里楼主就提供一下vista的bootmgfw.efi，需要的可以拿去
#注意，不是所有电脑主板都要求此文件才能UEFI启动win7/vista安装，已知vmware不需要
![](http://pan.baidu.com/s/1o835ADO
由于换了新pc，vista镜像找不到了[汗] 明天再继续教程，我去下载一下
把之前提取的bootmgfw.efi重命名为bootx64.efi，放入安装盘\EFI\Boot中（没有就新建）
然后镜像就准备好了，可以写入安装介质了
现在我们再次进入winpe，像上次一样为EFI分区分配盘符
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/90e26e25ab18972b5104996aefcd7b899f510a4d.jpg)
***
然后把EFI分区格式化（FAT32）
#确认之前已备份EFI文件夹
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/e4361a1fd21b0ef4621001fed4c451da83cb3e8f.jpg)
接下来重启，从vista安装介质启动
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/e1b0ca355982b2b7c2a2a26438adcbef77099b42.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/edc03e83b2b7d0a21ff49f3dc2ef76094a369a42.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/09a06e22dd54564ed4677f99bade9c82d0584f01.jpg)
正常安装vista
#注意别选错分区，别把win10覆盖了；esp/msr/recovery在vista安装程序里是隐藏的
#可能会提示你“不是推荐的分区顺序”，这并不影响安装，确定即可
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/6e29c4cd7cd98d101d299691283fb80e79ec9082.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/4903f7539822720eed1f785a72cb0a46f01fabb7.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/0f36b2638535e5ddce3d207f7fc6a7efcf1b6276.jpg)
自动重启进入第二阶段安装（某些机型UEFI引导vista速度比较慢，会在bootmgr卡一会儿）
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/d1d7f0dca144ad3455c80027d9a20cf430ad8514.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/4c23f62297dda144a67eeb12bbb7d0a20df48614.jpg)
***
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/0fbe47a5462309f74bb62ab27b0e0cf3d5cad6af.jpg)
进桌面
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/4903f7539822720ed747625a72cb0a46f01fabff.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/f9ccfc514fc2d562a7a1504dee1190ef74c66cde.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/edbfb61273f08202d119119f42fbfbeda9641bf8.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/f20f24176d224f4af510f3b300f790529a22d1ff.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/16baf559d109b3dede1664c8c5bf6c81820a4cde.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/d01b11c7a7efce1bb46b486aa651f3deb68f65c7.jpg)
重启进pe，依然挂载EFI分区，给他分配盘符
然后打开，你会看到一个新的EFI文件夹，建议备份一下
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/cca0f3eff01f3a2900245a6e9025bc315e607c93.jpg)
把之前提取的win8/10的EFI文件夹中的Microsoft文件夹改名，然后复制到现在的EFI分区\EFI下
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/7d9932fab2fb4316a0ddf4da29a446230bf7d342.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/150fd5fa43166d2281b59b344f2309f79252d242.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/e9f52b096e061d95bf6dbe9872f40ad163d9ca59.jpg)
打开Bootice（一般PE都自带），切换到UEFI选项卡
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/6e29c4cd7cd98d100ea58591283fb80e7aec9016.jpg)
***
打开“修改启动序列”
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/89c917ce3bc79f3dae7d6d90b3a1cd11708b29e3.jpg)
***
把现有的Windows Boot Manager改名为Windows Vista，然后保存当前启动项设置
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/c7f5c68a87d6277f3590bb9821381f30eb24fc82.jpg)
然后点击添加，打开刚才复制进EFI分区的win8/10相关启动文件里的bootmgfw.efi（本例中在ESP分区\EFI\win10\boot\bootmgfw.efi
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/3b006dd062d9f2d3ede5ac4fa0ec8a136127cc94.jpg)
***
把名称改一下，然后调整一下顺序，最后保存
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/03e20a234f4a20a488f6b46799529822700ed098.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/bd0ec850f3deb48fa9782a7ef91f3a292cf57876.jpg)
重启，进入UEFI BIOS设置，就可以选择启动哪个系统了
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/d8d6150f0cf3d7caaf99b4d6fb1fbe096a63a91d.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/1976d5b6d0a20cf43561757f7f094b36aeaf9996.jpg)
***
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/92ef69f51bd5ad6eb5aaee4a88cb39dbb7fd3c30.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/fa55aa10728b4710e056776ccacec3fdfd03230e.jpg)
***
（我不知道为什么这里蜜汁多了一项）
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/b2ebd9086b63f624b312cca38e44ebf81b4ca33d.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/e9f52b096e061d95bb5fc29872f40ad163d9ca6f.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/833aa4fcfc03924588b214af8e94a4c27c1e2504.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/ab0c7d4d510fd9f908b4a0c92c2dd42a2a34a4e1.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/ec5b49dca3cc7cd9878fc1793001213fba0e91e1.jpg)
不过这样做成的双引导，必须通过BIOS选择系统
两个系统下都只识别Windows Vista，不过不影响
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/3b7df9500fb30f2435bb18a3c195d143ac4b0366.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/0253be32c895d143d1ab11837af0820258af07a2.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/bb19cc65034f78f0712f6e5370310a55b2191c5b.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4970355831/32fa6bf2d7ca7bcbd8d9338fb7096b63f424a8e2.jpg)
如果觉得不方便，可以使用Clover、Grub等第三方引导器来引导不同的bootmgfw.efi，达到双引导的效果[哈哈]
教程到此结束
