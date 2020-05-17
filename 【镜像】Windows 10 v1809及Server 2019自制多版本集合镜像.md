我再也不相信微软了[冷] 说好的v1809的灾难不会重演，这两天听说又推了补丁把自家surface book搞蓝屏了。。。
然而集合镜像还是要（重）做的[滑稽] 
更新日志：
所有镜像版本更新至17763.107（修复升级时文件可能被删除的bug）
删去hyper-v server镜像（官方迟迟不更新至17763.107，都等了几周了）
增加Windows Server v1809镜像（即Windows Server Semi-Annual Channel 半年更新通道，有标准版和数据中心版共2个版本，无GUI桌面体验版本）
全版本集合镜像改用SWM分卷压缩（因为太大了），客户端版和服务器版仍使用esd压缩

这次集合镜像依然由原版镜像制作，仅压制、合并install.wim，未做任何改动。系统版本为17763.107。
win10和server的2个合集的install文件使用esd压缩，而win10+server的全版本合集镜像由于17763.107版本体积变大的缘故，使用esd压缩也超出了4GB的大小，所以改为SWM分卷压缩，虽然体积较大，但是每个文件都控制在了4GB内。3个镜像均支持FAT32的存储介质；刻录方面，除了第三个超过标准DVD需要双层DVD-DL外，1、2均支持4.7G DVD刻录
分为3个版本（注：文件名我标注的是10月更新版本，因为17763.107镜像是10月底编译的，msdn镜像名好像还是标注的9月更新，实际上官方镜像是11月发布的）：
1.Windows 10 v1809 多版本合集
包含家庭版、家庭中文版、家庭单语言版、教育版、企业版、专业版、专业教育版、专业工作站版、适用于虚拟桌面的企业版、企业版2019LTSC 共10个版本
文件名：cn_windows_10_client_editions_version_1809_rs5_refresh_updated_oct_2018_x64_dvd.iso
大小：3.93GB
WIM卷列表：
1.Core (Client)
2.CoreCountrySpecific (Client)
3.CoreSingleLanguage (Client)
4.Education (Client)
5.Enterprise (Client)
6.Professional (Client)
7.ProfessionalEducation (Client)
8.ProfessionalWorkstation (Client)
9.ServerRdsh (Client)
10.EnterpriseS (Client)
Wim卷名称：
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5972802200/fcc53b6134a85edfc590699744540923dc54755f.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5972802200/512bceed8a136327b52756879c8fa0ec0afac7b6.jpg)

2.Windows Server 2019 & Windows Server v1809 多版本合集
包含Server Essentials 2019、Server Standard Core 2019、Server Standard 2019（桌面体验）、Server Datacenter Core 2019、Server Datacenter（桌面体验）2019、Server Standard Core v1809、Server Datacenter Core v1809 共7个版本
文件名：cn_windows_server_2019_and_v1809_editions_version_1809_rs5_refresh_updated_oct_2018_x64_dvd.iso
大小：3.97GB
WIM卷列表：
1.ServerSolution (Server)
2.ServerStandard (Server Core)
3.ServerStandard (Server)
4.ServerDatacenter (Server Core)
5.ServerDatacenter (Server)
6.ServerStandardACor (Server Core)
7.ServerDatacenterACor (Server Core)
WIM卷名称：
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5972802200/0f36b2638535e5ddd46f326b7bc6a7efcf1b623c.jpg)

3.Windows 10 v1809、Server 2019 & Server v1809 多版本合集
包含 Windows 10 家庭版、家庭中文版、家庭单语言版、专业版、专业教育版、专业工作站版、教育版、企业版、适用于虚拟桌面的企业版、企业版2019LTSC、Server Essentials 2019、Server Standard Core 2019、Server Standard 2019（桌面体验）、Server Datacenter Core 2019、Server Datacenter（桌面体验）2019、Server Standard Core v1809、Server Datacenter Core v1809 共17个版本
文件名：cn_windows_client_and_server_editions_version_1809_rs5_refresh_updated_oct_2018_x64_dvd_dl.iso
（网盘中为7z分卷压缩文件2个）
大小：6.50G
WIM卷列表：
1.Core (Client)
2.CoreCountrySpecific (Client)
3.CoreSingleLanguage (Client)
4.Education (Client)
5.Enterprise (Client)
6.Professional (Client)
7.ProfessionalEducation (Client)
8.ProfessionalWorkstation (Client)
9.ServerRdsh (Client)
10.EnterpriseS (Client)
11.ServerSolution (Server)
12.ServerStandard (Server Core)
13.ServerStandard (Server)
14.ServerDatacenter (Server Core)
15.ServerDatacenter (Server)
16.ServerStandardACor (Server Core)
17.ServerDatacenterACor (Server Core)
WIM卷名称：
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5972802200/dedb600928381f302c831a1da4014c086c06f0e6.jpg)
![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5972802200/141351d02f2eb938b5d5ed46d8628535e4dd6f3b.jpg)

链接楼下放[滑稽]（其实还是上次的链接）
***
emmm不改一下标题怕不是大家都以为是老的那个版本 这个是更新过的[狂汗]
@Longhorn4093
***