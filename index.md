---
layout: single
title: "Home"
toc: true
url: /
---
#### **Introduction to SSS&SDS Group**

<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
<title>jQuery响应式Banner图片轮播代码</title>

<link rel="stylesheet" href="css/style.css" />

</head>
<body>

<div class="c-banner">
	<div class="banner">
		<ul>
			<li><img src="img/lunbo1.jpg"></li>
			<li><img src="img/lunbo2.jpg"></li>
			<li><img src="img/lunbo3.jpg"></li>
		</ul>
	</div>
	<div class="nexImg">
		<img src="img/nexImg.png" />
	</div>
	<div class="preImg">
		<img src="img/preImg.png" />
	</div>
	<div class="jumpBtn">
		<ul>
			<li jumpImg="0"></li>
			<li jumpImg="1"></li>
			<li jumpImg="2"></li>
		</ul>
	</div>
</div>

<script type="text/javascript" src="js/jquery.min.js"></script>
<script type="text/javascript">
//定时器返回值
var time=null;
//记录当前位子
var nexImg = 0;
//用于获取轮播图图片个数
var imgLength = $(".c-banner .banner ul li").length;
//当时动态数据的时候使用,上面那个删除
// var imgLength =0;
//设置底部第一个按钮样式
$(".c-banner .jumpBtn ul li[jumpImg="+nexImg+"]").css("background-color","black");


</script>
</body>
</html>
#### **News**

- Our paper "MORE<sup>2</sup>: Morphable Encryption and Encoding for Secure NVM" is is accepted by [ICCAD 2021](https://iccad.com/index.php). Congratulations to [Wei Zhao](https://thiszw.top).  
- Our paper "Better atomic writes by exposing the flash out-of-band area to file systems" is accepted by [LCTES 2021](https://pldi21.sigplan.org/home/LCTES-2021#event-overview). Congratulations to Hongwei Qin.  
- Our paper "Improving the energy efficency of STT-MRAM based approximate cache" is accepted by [DATE 2021](https://www.date-conference.com/). Congratulations to [Wei Zhao](https://thiszw.top).  
- Our paper "MorLog: Morphable Hardware Logging for Atomic Persistence in Non-Volatile Main Memory" is accepted by [ISCA 2020](https://iscaconf.org/isca2020/). Congratulations to Xueliang Wei.  
