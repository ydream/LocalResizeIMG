LocalResizeIMG
==============

# 前端HTML5本地压缩图片，兼容移动设备IOS,android。


## 概述
* 通常压缩图片需要上传到后端，由后端处理。
* 但是如果要上传的图片很大，特别是手机当场拍摄下来的照片（约2M+），那样效率会很低，用户也不会愿意等待。
* 现在能够由前端本地压缩的话，效率将会极大的提升。

## BUG修复
* 修复android下压缩无效果的问题
* 修复IOS压缩图片扭曲的问题。
* 微信的话... 经过测试，目前新版本都支持触发上传了，大赞！XD

## 使用方法
具体详情请查看 源代码，或者 demo。
```
	$('input:file').localResizeIMG({
	     width: 100,
	     quality: 0.1,
	     // before: function () {},
	     success: function (result) {
	     var img = new Image();
	     img.src = result.base64;

	     $('body').append(img);
	     console.log(result);
	     }
	 });
```

## PS
这是8个月前的测试文章的延伸，[点我去看看](http://my.oschina.net/hzplay/blog/160806)。


> ##### 技术： jquery
> ##### 时间： 2014年5月
> ##### 源码： [Guthub](https://github.com/think2011/LocalResizeIMG)
