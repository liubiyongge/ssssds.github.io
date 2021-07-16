---
layout: default
title: "Home"
toc: true
url: /
---
#### **Introduction to SSS&SDS Group**



<head>
    <meta charset="utf-8">
    <title>picplay</title>
    <style>
        #divout {
            max-width: 1000px;
            position: relative;
            margin: 0 auto;
        }

        .imgdiv img {
            width: 80%;
        }

        .imgdiv {
            display: none;
        }

        .dotdiv {
            text-align: center;
            position: absolute;
            width: 100%;
            bottom: -30px;
        }

        .dot {
            width: 16px;
            height: 16px;
            display: inline-block;
            background: #bbbbbb;
            border-radius: 10px;
            margin: 0 12px;
        }

        .title {
            font-size: 18px;
            color: #f2f2f2;
            position: absolute;
            text-align: center;
            font-weight: 700;
            width: 100%;
            bottom: 10px;
        }

        .active {
            background-color: #717171;
        }

        #arrow {
            position: absolute;
            top: 50%;
            margin-top: -30px;
            width: 100%;
            opacity: .3;
            transition: opacity 2s;
        }

        #divout:hover #arrow {
            opacity: .9;
        }

        #arrow img {
            cursor: pointer;
        }

        .imgdiv {
            animation: fade 1.5s;
        }

        @keyframes fade {
            from {
                opacity: .3;
            }

            to {
                opacity: 1;
            }
        }
    </style>
</head>

<body>
    <!--    div#divout>(div.imgdiv>img+div.title{标题文本$})*4 +(div.dotdiv>span.dot*4)-->
    <div id="divout">
        <div class="imgdiv" style="display: block">
            <img src="/assets/img/group1.jpg" height="80%" width="80%" alt="">
            <div class="title">Group Party</div>
        </div>
        <div class="imgdiv">
            <img src="/assets/img/award.png" height="80%" width="80%" alt="">
            <div class="title">OlympusMons Award</div>
        </div>
        <div class="imgdiv">
            <img src="/assets/img/group1.jpg" height="80%" width="80%" alt="">
            <div class="title">标题文本3</div>
        </div>
        <div class="imgdiv">
            <img src="/assets/img/group1.jpg" height="80%" width="80%" alt="">
            <div class="title">标题文本4</div>
        </div>
        <div class="dotdiv">
            <span class="dot active"></span>
            <span class="dot"></span>
            <span class="dot"></span>
            <span class="dot"></span>
        </div>
        <div id="arrow">
            <img src="https://upload-images.jianshu.io/upload_images/24975120-26bbb7165d5c274e.png?imageMogr2/auto-orient/strip|imageView2/2/w/178/format/webp" alt="" width="60" onClick="picplay(false)">
            <img src="https://upload-images.jianshu.io/upload_images/24975120-2d3152494090caaf.png?imageMogr2/auto-orient/strip|imageView2/2/w/178/format/webp" width="60" alt="" align="right" onClick="picplay(true)">
        </div>
    </div>

</body>

<script>
    var imgIndex = 0;
    var imgDivArr = document.getElementsByClassName("imgdiv");
    var dotArr = document.getElementsByClassName("dot");
    /**
     *  播放图片
     *  参数r：是否正放，若为true，正放。若为false，倒放
     */
    function picplay(r) {
        for (let i = 0; i < imgDivArr.length; i++) {
            imgDivArr[i].style.display = "none";
            dotArr[i].className = "dot";
        }
        if (r) {
            imgIndex++;
            imgIndex = (imgIndex >= imgDivArr.length) ? 0 : imgIndex;
        } else {
            imgIndex--;
            imgIndex = (imgIndex < 0) ? imgDivArr.length - 1 : imgIndex;
        }
        imgDivArr[imgIndex].style.display = "block";
        dotArr[imgIndex].className = "dot active";
    }
    setInterval(picplay, 3000, true);

</script>

#### **News**

- Our paper "MORE<sup>2</sup>: Morphable Encryption and Encoding for Secure NVM" is is accepted by [ICCAD 2021](https://iccad.com/index.php). Congratulations to [Wei Zhao](https://thiszw.top).  
- Our paper "Better atomic writes by exposing the flash out-of-band area to file systems" is accepted by [LCTES 2021](https://pldi21.sigplan.org/home/LCTES-2021#event-overview). Congratulations to Hongwei Qin.  
- Our paper "Improving the energy efficency of STT-MRAM based approximate cache" is accepted by [DATE 2021](https://www.date-conference.com/). Congratulations to [Wei Zhao](https://thiszw.top).  
- Our paper "MorLog: Morphable Hardware Logging for Atomic Persistence in Non-Volatile Main Memory" is accepted by [ISCA 2020](https://iscaconf.org/isca2020/). Congratulations to Xueliang Wei.  

