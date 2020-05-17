# 【教程+直播】LineageOS x86\_64从安装到ROOT

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/7a075d86e950352a687defe25f43fbf2b3118b36.png)

先下载一下需要的东西 LineageOS 14.1 x86\_64:\[https\]osdn点net/projects/android-x86/downloads/68670/cm-x86\_64-14.1-r2.iso/

1、安装 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/4c0056accbef76098911ac7422dda3cc7dd99e3c.png) 这里这样选 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/5ee3ed83b9014a90a4517356a5773912b11beee7.png) SATA

硬盘大小随你便，挂载镜像，{开启3D加速【重要，不然安装好进不去GUI】}，不！要！用！UEFI！！！！！ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/c2d2a8fd1e178a82f61d4b4bfa03738da877e829.png) 选择第三个 好像XP？？？？？

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/91fdd4df9c82d15839006d5a8c0a19d8be3e4254.png) 这里等个二三十秒的样子按＋，选择这个，OK

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/92ef69f51bd5ad6efe0c50018dcb39dbb4fd3c5c.png) 选择No，当然你有技术你可以UEFI引导使用GPT，但是我没找到这玩意UEFI Grub的方法

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/17d876dea9ec8a131542600bfb03918fa2ecc0f2.png) 这里像我这样选择 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/bb19cc65034f78f0b5eead1875310a55b1191c6c.png)

这里直接回车 !\[\]\([https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/ef371e300a55b319ac2db59e4fa98226cdfc177d.png](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/ef371e300a55b319ac2db59e4fa98226cdfc177d.png) Bootable可引导 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/f7b124a88226cffc52fa8859b5014a90f403ea7a.png) 选择Write，输入yes回车 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/3b1833e636d12f2e7411988b43c2d5628435683e.png)

选择Quit，选择SDA1回车 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/f0a59f188618367a827e493622738bd4b11ce55f.png) 当然ext4 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/c6ec517bdab44aed77558f0fbf1c8701a08bfb33.png) Yes ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/f6f45df23a87e9509d28c2871c385343faf2b417.png) Yes ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/c0fe7ed9bc3eb135ca288150aa1ea8d3ff1f4467.png) yes ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/e9835e13b31bb051acb082c33a7adab448ede0be.png) 然后坐和放宽 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/7b33f83cf8dcd100b714c9ca7e8b4710bb122f41.png)

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/7add4af4e0fe99255e0059bb38a85edf8fb171c6.png) 拔盘，Reboot重启

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/141351d02f2eb938505c4919d9628535e4dd6f19.png) 第一次启动需要很长很长很长很长的时间，大家等我弄好吧。我现在用的没存干净快照

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/7a738e51352ac65cb4bd5998f7f2b21191138a92.png) cHINESE在最底下 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/f9e6affdc3cec3fdf274999eda88d43f85942783.png) 使用新设置 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/f86dce004c086e067f5b01a00e087bf408d1cb5b.png)

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/0b0f9cecab64034f4fe1fbeda3c379310b551d25.png) 这样正常，确定即可

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/b6f7148ca9773912fa22bd8af4198618347ae2ce.png) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/ab0c7d4d510fd9f9587a6d82292dd42a2a34a4e5.png) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/7a738e51352ac65cb11b5e98f7f2b21192138a30.png) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/4aa1d418ebc4b7457dde8ffdc3fc1e1788821583.png) 这里要拉到底部 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/f9f52d91f603738dee0034c9bf1bb051fa19ec8c.png) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/edc03e83b2b7d0a2bdd73c76c7ef76094a369a30.png) 完成之后有个选择默认应用，选择下面那个T什么的，点击始终

下载SuperSU ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/1292b7170924ab188854dadc39fae6cd79890b8b.png) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/a9d0df98a9014c083098134e067b020879f4f4ab.png) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/2b9791256b600c330efde523164c510fdbf9a14e.png)

下载完成后，Alt+F1进入CLI，按照我这样输入命令

```text
mkdir /sdcard/Download/su
cd /sdcard/Download/su
unzip ../SuperSU-v2.82-201705271822.zip
cd /system/xbin
cp /sdcard/Download/su/x64/su .
chmod 4751 su
su --install
su --daemon
```

这里如果有在CLI和GUI中闪来闪去的Bug，重启接着你刚刚执行完的代码后面来

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/f6f45df23a87e950af56d4871c385343f9f2b489.png) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/b7f7f68ea0ec08fa3ddb344c55ee3d6d57fbda73.png) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/3304e5035aafa40f6606e936a764034f7af01909.png) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/91acabbe6c81800afea3aee5bd3533fa808b4788.png) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/c2f63daea40f4bfbd510b9bf0f4f78f0f5361809.png) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/e8279a1e4134970ac1ab37c499cad1c8a5865d72.png) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/891e72cf36d3d539202028283687e950342ab035.png) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/4f47682542a7d933ede9c398a14bd11371f00188.png) 这里会有一个警告，确认 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/4fd025a6d933c895f7a5bf90dd1373f080020072.png) 然后返回在双击Superuser.apk，安装。

然后打开Supersu，如果要求更新SU文件，继续，选择常规方式安装，安装完成后重启 教程结束!

彩蛋：SuperSU可以开启专业版，在设置拉到底下有个启用专业版，勾上 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5796154683/f3ed8cc5b74543a9b63ed72712178a82b801142c.png) Free的伪专业版

