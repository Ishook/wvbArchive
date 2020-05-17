# win10 TP缺少api-ms-xxx.dll的解决办法

![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/5536755818/891e72cf36d3d5395eb7fb083187e950372ab06d.jpg)

首先，能肯定的是，报缺少哪个dll就补上哪个。 但是，有些坑的是，那些dll补得版本还不一定能一样，例如说a.dll补得可能是win8的，b.dll可能补得是win10的，如果搞错了，打开应用程序会出现0x000007b或者无法注册dll。 所以早上花了几个小时整理了一些能够兼容的dll：[http://pan.stnts.com/s/FFQnf6w注册完这些dll能够解决一些程序缺少dll的情况。](http://pan.stnts.com/s/FFQnf6w注册完这些dll能够解决一些程序缺少dll的情况。) 但是，如果你打开程序还是提示缺少dll，请自己去百度或者去iso提取缺少的dll，如果无法注册，或者注册完以后在打开程序提示0x000007b错误的话，就需要换一个版本的dll了。

哦另外，如果补64位补丁死活不行，可以去补32位的，只要成功即可\[滑稽\]

