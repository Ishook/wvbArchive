# USB Vista10

要求U盘最少32GB，2.0\[滑稽\] 下载地址：链接：!\[\]\([http://pan.baidu.com/s/1hszblXE](http://pan.baidu.com/s/1hszblXE) 密码：iybn 说明：下载 vista10.7z.001及vista10.7z.002，把这两个压缩包放在同一目录解压，就会得到一个VHD镜像。Tools.zip内有必备的工具。 首先，把U盘格式化为NTFS格式。 然后安装 Tools.zip 内的“EasyBCD 2.3 Beta - Build 197” 打开EasyBCD，进入“BCD部署”，在“分区”这一项选择你的U盘，点击“安装BCD” ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5052257913/d2acb608b3de9c826b9af2546581800a1bd84367.jpg)

完成后，先不要关闭EasyBCD 然后，把 vista10.7z.001和vista10.7z.002 放在同一目录，打开其中一个，解压到本地磁盘。 把解压在本地磁盘的 “vista10.vhd” 复制到你的U盘，复制完成后，解压Tools.zip 内的“wcontig”。 打开wcontig，点击“添加” ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5052257913/553a51d2d539b6005985736ce050352ac45cb793.jpg)

然后选择你刚刚复制到U盘的VHD文件 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5052257913/d0a6ff23720e0cf391cc30200346f21fbf09aa23.jpg)

点击wcontig的“ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5052257913/dc76b659ccbf6c8130455233b53eb13531fa40f4.jpg) 结果为“无碎片”就是好了。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5052257913/c7f5c68a87d6277f82cf4ce321381f30eb24fc05.jpg) 这里先解压在本地磁盘在复制进U盘就是为了“无碎片” 打开EasyBCD，编辑U盘的引导。 如果已经把EasyBCD关掉了，别急，重新执行这一步↓ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5052257913/3b7df9500fb30f24a81397d8c195d143af4b0351.jpg)

这里会弹出一个窗口，点“是” ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5052257913/ebecf02ad40735fa020e346297510fb30d240860.jpg)

然后点击EasyBCD的“添加新条目” ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5052257913/222d95d2572c11df802adaf86a2762d0f503c263.jpg) ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5052257913/a6391c889e510fb3e896124cd033c895d3430c57.jpg)

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5052257913/f0a59f188618367ad7541b0627738bd4b11ce505.jpg)

选择好镜像后，随便给“名称”改个名字，点“添加条目” ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5052257913/4fd025a6d933c89538b3ffa0d81373f080020015.jpg) 使用部分 第一次启动后，系统会自动安装驱动（不一定能打全，桌面有万能驱动，但这时候先不要使用万能驱动） 安装驱动后，会让你重启，这时不要重启，双击桌面的“EWF”，点击里面的“EWF Save” 不要重启，双击桌面的""EWF"" ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5052257913/65ebf2cbd1c8a7867bc026d56e09c93d72cf507c.jpg) @qjy妈妈我爱你 来看看\[滑稽\] 使用 万能驱动助理 时，要把""其他设置""的""解压位置""改成 R:\Drivers 并且勾选上 ""安装完成后删除已解压驱动文件"" 最好一次只安装一个驱动，防止EWF内存写满了，并且最好在确定只有在几台或一台电脑使用时，才安装驱动。 还有，最好把浏览器等软件的临时目录改在内存盘\(R盘\) 本系统自带一个大小为1gb的内存盘。 由于使用了EWF，对系统的写入操作是不保存的，所以在安装完驱动后或者想保存本次写入操作时，都要双击桌面的""EWF""，点击里面的“EWF Save”进行保存。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5052257913/89e3183f6709c93dc12c652c963df8dcd3005400.jpg) 使用效果图\[滑稽\]@lsqsjz ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5052257913/11c9419659ee3d6d4b67d5104a166d224d4adeb9.jpg) @什么事人 \[滑稽\]来看看

