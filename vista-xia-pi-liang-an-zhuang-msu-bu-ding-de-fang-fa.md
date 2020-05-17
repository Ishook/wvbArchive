# Vista下批量安装msu补丁的方法

首先要暂时关闭UAC，打开msconfig，在工具选项卡下，运行禁用uac的工具，然后重启 接下来，把msu放在一个文件夹里面，按住shift右键文件夹，在此处打开命令提示符 输入命令行： for %%i IN \(\*.msu\) DO wusa %%i /quiet /norestart 等待它自己一个个安装 安装完之后，可以到msconfig的工具选项卡底下，运行启用uac来恢复uac，然后重启完成更新的配置

打补丁时的效果： ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5533963902/fefd0c62f6246b6097b87bbce0f81a4c530fa2be.jpg)

注意，对于像IE9、WU Agent这样的非msu补丁，以及解压成cab格式的补丁，则不适用于这种方法。

