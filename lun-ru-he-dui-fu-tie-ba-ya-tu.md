# 论如何对付贴吧压图

手机上的贴吧可能会遇到贴吧压图的情况,当然我的kindle也是。最近我找到了一种应付方法。 1.打开wap版贴吧,过程不再赘述。 2.打开要看的帖子,点击欲看的图片,会跳转到一个只有那个图片的页面。 3.这个页面的图是压过的,横向分辨率被压到400,所以可能很糊。当然如果图片本来就不大,可能就不会压了。 注意地址栏,你会发现一段“size=b400\_2000”\(看不到的话把网址拖动一点就行了\),就是这个东西限制了图片尺寸到400\*2000。 4.把这两个值改得足够大,就可以看到完整尺寸的图了。但是不可大于65535,不然会出现问题。 现在的图已经基本可看了。但是仔细看一看,仍会发现画质比原图略有降低。\(不仔细看并无影响\) 5.就在“size=”左边一点有个“quality=80”,把80改成1100即可。 然后你就获得真正的原图啦! extra.小实验:\(1\)把quality改成0,发现糊得已经很容易看出问题了,结果改成1,比0还糊!糊到什么程度呢,像突然被戴上高度老花镜一样。。。 \(2\)“quality=”左边还有一个“wapp”,用途不明。我把它删了也没变化。 要不是@C型钢7 提醒我都忘了发图了\[滑稽\]特地感谢一下\[滑稽\] 3楼图 ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4946665487/7add4af4e0fe992533a4071c3da85edf8fb171c3.jpg) 4楼图（被百度压了的图） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4946665487/112ee6ca39dbb6fd83a58b6a0024ab18952b37f1.jpg) 6楼图（更改分辨率限制） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4946665487/f47beb5594eef01fb1b67689e9fe9925be317dd5.jpg) 8楼图（更改清晰度限制） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4946665487/1292b7170924ab1843dc887b3cfae6cd79890bad.jpg)

9楼图（最终效果） ![](https://wvbarchive.s3-ap-northeast-1.amazonaws.com/4946665487/f6f45df23a87e95061e79d2019385343f9f2b4fb.jpg)

