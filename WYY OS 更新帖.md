由于原贴太乱，现重开一贴更新，原贴地址：p/5541766523
Rev 2.8 更新
1、以后WYY OS 弃用PMF安装，使用自制安装器
2、优化保险箱打开方式，使用软链接（重要！安全性增加120%）
***
2l 链接
3l 安装方法
打开下载下来的zip压缩包，打开其中的bat文件夹
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6032479193/d17bc7ed08fa513dc0b7c11b306d55fbb0fbd9c8.jpg)

里面有几个ini，全部按照下面的要求配置
1 要安装到的磁盘（第一块磁盘为1，以此类推），输出在bat\d.ini里
2 要安装到的分区 (第一个分区为1,以此类推)，输出在\bat\p.ini里
3 分区大小 单位mb 你做一个限制，最小1024mb。输出在\bat\rs.ini里
4 目标计算机系统位数，输出在\bat\bit.ini里，为64或86

配置完毕打开im.bat
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6032479193/89e3183f6709c93d031da332923df8dcd3005479.jpg)

如果配置正确会弹出上图所示的小窗口，请检查其中的分区是否是你要安装到的分区，如果是，按开始按钮开始安装。
安装结束后就可以进入安装后的磁盘进行使用了。
***
打开保险箱时会弹UAC，请允许

保险箱打开后根目录会出现一个叫保险箱的目录
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6032479193/833aa4fcfc039245a89848ca8a94a4c27c1e253f.jpg)

打开即可使用。
要关闭保险箱时请打开保险箱内的Manager.bat，点击关闭保险箱即可
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/6032479193/91b7ca4ad11373f01d85c65aa90f4bfbf9ed04b6.jpg)
***
@2006bt @Longhorn4093 @孙必林
WYY OS 4.0将会脱离畸形文件夹加密，转用更加安全的文件系统级加密方式