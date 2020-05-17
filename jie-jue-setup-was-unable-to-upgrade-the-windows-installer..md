# 解决“Setup was unable to upgrade the Windows Installer.“

你一定见过。。。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5304062172/42fc1cf50ad162d94a11eb2f1adfa9ec8b13cd78.jpg)

办法超级简单：下载以下msi文件，启动到目录服务恢复模式，然后把msi文件拿给虚拟机安装。 [https://pan.baidu.com/s/1pLFkyQR](https://pan.baidu.com/s/1pLFkyQR)

此办法在Longhorn 3718和XP 2498上均测试通过。不过，不保证这样强行安装的VMware Tools可以工作得完全正常，我甚至也不能保证它不会导致系统崩溃。使用它带来的损失我概不负责，使用前建议保存快照。 我这个只装主程序，不会装驱动，如果要装驱动不能靠2楼的东西，你可以下载另一个专门的补丁包 [https://pan.baidu.com/s/1kVBQM3t](https://pan.baidu.com/s/1kVBQM3t) 自己多拿几个系统试验了一下，有几点跟大家说明一下： 1.VMware Tools安装用我这个办法我还没失败过。不过有时候VMware Tools并没有开机启动（虽然右下角仍然有图标）。这种情况下，请手动运行vmtoolsd.exe。 2.VMware Tools可能提示相关服务没有打开或者有什么别的问题，实验下来发现是不影响的，忽略即可。 3.如果想要使用诸如自动调节分辨率之类的功能，必须另安装VMware显驱，该显驱不会被本帖的安装包自动装上，要安装请移步[https://pan.baidu.com/s/1kVBQM3t。](https://pan.baidu.com/s/1kVBQM3t。) 如果各位有什么使用问题可以问我，我尽可能帮忙。 虽然我前面发了那么大一段免责声明，但是其实失败的概率应该很小。现在已经证明这些功能可以使用： ·主机和虚拟机共享剪贴板； ·虚拟机自动根据VMware窗口大小调整自己的分辨率； ·直接把文件拖拽复制到虚拟机； ·通过虚拟机外的“关闭虚拟机”按键进行软关机（如果没装tools则会硬关机）； ·Unity模式！ 我想应该还不止这么多。

展示图： XP 2495的常规办法安装： ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5304062172/e3381bd88d1001e9c344f12db30e7bec55e7978a.jpg) 用我的办法安装：分辨率可以更改！ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5304062172/43bb1ff1f736afc30e40da47b819ebc4b64512bd.jpg) Longhorn 3683的常规办法安装： ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5304062172/c7f5c68a87d6277f0b3ed71a23381f30e824fcde.jpg) 用我的办法安装：成功打开Unity！！ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5304062172/c722407e9e2f0708b086d022e224b899a801f203.jpg)

你一定见过。。。 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5304062172/42fc1cf50ad162d94a11eb2f1adfa9ec8b13cd78.jpg)

办法超级简单：下载以下msi文件，启动到目录服务恢复模式，然后把msi文件拿给虚拟机安装。 [https://pan.baidu.com/s/1pLFkyQR](https://pan.baidu.com/s/1pLFkyQR)

此办法在Longhorn 3718和XP 2498上均测试通过。不过，不保证这样强行安装的VMware Tools可以工作得完全正常，我甚至也不能保证它不会导致系统崩溃。使用它带来的损失我概不负责，使用前建议保存快照。 我这个只装主程序，不会装驱动，如果要装驱动不能靠2楼的东西，你可以下载另一个专门的补丁包 [https://pan.baidu.com/s/1kVBQM3t](https://pan.baidu.com/s/1kVBQM3t) 自己多拿几个系统试验了一下，有几点跟大家说明一下： 1.VMware Tools安装用我这个办法我还没失败过。不过有时候VMware Tools并没有开机启动（虽然右下角仍然有图标）。这种情况下，请手动运行vmtoolsd.exe。 2.VMware Tools可能提示相关服务没有打开或者有什么别的问题，实验下来发现是不影响的，忽略即可。 3.如果想要使用诸如自动调节分辨率之类的功能，必须另安装VMware显驱，该显驱不会被本帖的安装包自动装上，要安装请移步[https://pan.baidu.com/s/1kVBQM3t。](https://pan.baidu.com/s/1kVBQM3t。) 如果各位有什么使用问题可以问我，我尽可能帮忙。 虽然我前面发了那么大一段免责声明，但是其实失败的概率应该很小。现在已经证明这些功能可以使用： ·主机和虚拟机共享剪贴板； ·虚拟机自动根据VMware窗口大小调整自己的分辨率； ·直接把文件拖拽复制到虚拟机； ·通过虚拟机外的“关闭虚拟机”按键进行软关机（如果没装tools则会硬关机）； ·Unity模式！ 我想应该还不止这么多。

展示图： XP 2495的常规办法安装： ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5304062172/e3381bd88d1001e9c344f12db30e7bec55e7978a.jpg) 用我的办法安装：分辨率可以更改！ ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5304062172/43bb1ff1f736afc30e40da47b819ebc4b64512bd.jpg) Longhorn 3683的常规办法安装： ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5304062172/c7f5c68a87d6277f0b3ed71a23381f30e824fcde.jpg) 用我的办法安装：成功打开Unity！！

