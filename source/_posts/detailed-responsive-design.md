---
title: 前端响应式详解
date: 2020-03-12 00:40:13
author: 前端时空-陈随易
tags: ["响应式", "布局", "响应式设计"]
categories: "CSS"
---

> 一两年以前，我发现，很多人都被响应式搞得很懵逼。
> 现在，我依然发现，还是有很多人，依旧被响应式搞得很懵逼。
> 所以，我也很懵逼。
> 到底是哪个环节出了问题，让这么多学习前端的同学对于这个响应式很懵逼呢？
> 我想，平时总是会百度过响应式这个关键词吧，数以万计的教程，难道就没有一个能让自己顿悟的？
> 所以，我不信，为了天下没有难学的编程，我打算继续为这万分之一添砖加瓦。

<!--more-->

## 什么是响应式？
很多人之所以对响应式很懵逼，最基本的一个原因就是，压根就不懂什么是响应式。
废话，要是懂的话，我还有啥好问的？
没错，你说得很有道理。
所以，我打算用下文，来详细讲解，什么是响应式。
任何行业，都喜欢创造术语，同样地，响应式就是其一。
所谓的术语，必然和专业，高深，冷酷，无情挂钩。
你想百般亲近它，但是它却对你不理不睬。
为了打破你们二者之间的僵局，我打算揭下响应式这一层神秘的面纱。
响应式：响应不同屏幕设备合适地展现网页效果的方式或着手段。
没错，不仅仅是方式，而且还有手段，请先对这个词有个印象，后面我们会和它，再次相遇。



![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/1.png)

我不知道，同学们在查找资料的时候，文章里是怎么解释响应式的。
可以看到，我这句解释，非常妙。

![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/2.png)

响应响应，何谓响应？我喊你，你回应我，这就是响应，响应了我喊你这件事。
我打你，你反过来打我。这不对，虽然这没有违背物理规律，但是这不够尊老爱幼。
那么同样的，我喊你，你回答：哎，哥，咋了？
你妈妈喊你，你回答：哎，妈，又怎么了？
你老爸喊你，你回答：哎，老爸，有啥事啊？
你老妹，老弟喊你，你回答：喊什么喊，一遍玩去，我忙着呢。
所以，从这里可以得知，什么是响应式？就是说，不同的屏幕，它不能一成不变地显示一样的内容，得根据屏幕大小，显示合适的内容。
记住合适这个词，你不能说你妈妈喊你，你也回答：哎，哥，咋了？对不对？
见人说人话，见鬼说鬼话，不然你行走江湖两行泪，痛苦不堪又受罪。
所以，要理解一个术语，咬文嚼字是有必要的。
其次，我们来看一下，这个不同屏幕的含义。
这个地方，很容易让人哭笑不得。
我遇到过不止一个同学，绞尽脑汁地在思考，如果用户缩放百分比，鼠标拖动屏幕调整大小，我该怎么响应式？
兄die!你的响应式是要适应天地万物，比孙悟空的七十二般变化还能变吗？
那我只能说一句：牛逼！
所以，这里要牢记，响应式并不是孙悟空，它所要适应的，就是那些，正常情况下的响应式。
那种非人类的用户，拿着浏览器，网页百分比调个不停，网页大小鼠标拖了个不亦乐乎，这种用户你留着他干嘛？留着他炒个青椒炒肉不放辣椒吗？
所以，同学们啊，你们是在花钱，花时间，花精力学代码啊，头脑要灵活一点啊！
一顿痛批之后，我们来总结一下：总结如上。

## 一个响应式板砖的响应式历程

扯了那么多，我相信，同学们最关心的还是这里。
no b b,show code.
同学们这种实事求是的精神，搞得我几度都想再多BB一下。
不过，为了同学们的前途着想，我决定，暂时先小声BB。

![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/3.png)

首先呢，我们从最简单的开始。
毕竟，我不想让大家一口吃个大胖子，更加不想让大家一口吃瘪。
更何况，吃个大胖子还是违法的。
为了广大胖友的利益，我们先来画一块板砖。

![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/4.png)

尽管我一直以来，都坚信我们的中国汉字，博大精深，源远流长。
但是，自从遇见了百度翻译，我没想到，原来我们的汉语拼音，更加博大精深！
```html
 /* 板砖div */
<div class="MLGB"></div>
```

```css
 /* 重置一下 */
* {
    padding: 0;
    border: 0;
    margin: 0;
    outline: 0;
    box-sizing: border-box;
}
 /* 板砖 */
.MLGB {
    width: 800px;
    height: 500px;
    background-color: antiquewhite;
}
```

![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/5.png)

没办法，我是一个相信缘分的人，天意如此，我也只能顺其自然。
所以呢，这就是一个普通的，有高度，有宽度的，div。
你说这div，它又长又宽，它像不像砖？

![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/6.png)

为了让大家更清楚地看到全貌，我们将浏览器整体调整一下。
那么，这么一调整呢，问题就来了。
大家发现没有，底部居然出现了可恶的横向滚动条！
什么鬼？！这一点都不响应式！
```css
 /* 重置一下 */
* {
    padding: 0;
    border: 0;
    margin: 0;
    outline: 0;
    box-sizing: border-box;
}
 /* 板砖 */
.MLGB {
    width: 100%;
    height: 500px;
    background-color: antiquewhite;
}
```
![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/7.png)

解决它，把宽度变成百分比，就，设置成100%好了。
完美，一个响应式的板砖，应天时地利，涅槃重生！
那么，同学们，响应式是不是很简单？
我们甚至有N种方法，让这个板砖响应式。
```css
 /* 重置一下 */
* {
    padding: 0;
    border: 0;
    margin: 0;
    outline: 0;
    box-sizing: border-box;
}
 /* 板砖 */
.MLGB {
    width: 1rem;
    height: 500px;
    background-color: antiquewhite;
}
```      
```javascript
document.documentElement.style.fontSize = window.innerWidth + "px";
```

![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/8.png)

没错，就是这么嚣张，直接1rem。
那么，这个1rem等于多宽呢？
就是我们的100%宽度，也就是等于，html标签里font-size设置的字体大小的值。
所以，1rem等于html根元素的font-size的数值大小。
不信的话，我们可以设置宽度为0.5rem。
```css
/* 板砖 */
.MLGB {
    width: 0.5rem;
    height: 500px;
    background-color: antiquewhite;
}
```     
![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/9.png)

一图胜千言，本文瞬间可以少写1000字，开心。
那么，除了rem，百分比，还有什么办法呢？
记住这一点，js是无所不能的。
```css
 /* 板砖 */
.MLGB {
    /* 宽度不见啦！ */
    height: 500px;
    background-color: antiquewhite;
}
```
```javascript
document.getElementsByClassName("MLGB")[0].style.width = window.innerWidth + "px";
```
![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/10.png)

所以大家看到没有，我们直接用万能的js，直接给板砖设置等于窗口内容的宽度，不就行了？
所以，大家还记得前面的那个词语，手段，吗？
不是你不会响应式，是因为，你的手段不够毒辣！
你百分百掌握着响应式的法术，却无法施展，为啥呢？你缺乏心法。
还好，我这有无数的心法，关注我，我教你心法。

## 情况当然没这么简单

真正的历练，才刚刚开始。

![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/11.png)

假设我们接到这样一个，开发天猫双十一主战场页面...的异想天开的任务。
```html
<div class="MLGB">
    <!-- 头部 -->
    <div class="header">
        欢迎大家来到，双十一天猫主会场！
    </div>
    <!-- 分会场入口 -->
    <div class="nav">
        <a class="box" href="##">鞋子</a>
        <a class="box" href="##">箱包</a>
        <a class="box" href="##">数码</a>
        <a class="box" href="##">服装</a>
        <a class="box" href="##">乐器</a>
        <a class="box" href="##">户外</a>
        <a class="box" href="##">家具</a>
        <a class="box" href="##">家具</a>
        <a class="box" href="##">影视</a>
        <a class="box" href="##">美食</a>
    </div>
</div>
```
```css
/* 搬砖 */
.MLGB {
    height: 500px;
    background-color: antiquewhite;
}
.header {
    height: 50px;
    line-height: 50px;
    font-size: 18px;
    color: #fff;
    text-align: center;
    background-color: #f97c7c;
}
.nav {
    height: 100px;
}
.box {
    display: block;
    width: 10%;
    float: left;
    height: 100px;
    line-height: 100px;
    text-align: center;
    text-decoration: none;
    font-size: 18px;
    border: 1px solid #ddd;
}
```    
![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/12.png)

我们刷刷刷，几个分会场入口就布局完了。
然后，我们一边欣赏这个10分钟之内创造的艺术品，一边品尝这我们前面的青椒炒肉不放辣椒的时候。
测试跑了过来...

![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/13.png)

鸡哥，鸡哥，出问题了！
嗯！你眼露杀气，在测试和他的手机之间，以每秒300赫兹的频率，来回扫描。
不，这不可能，我是一个合格的高级前端工程师，你这是什么手机？哼，我拿自己的瞧瞧。
于是，10秒钟后...
小李啊，你回去吧，这个BUG，我来解决。
```css
 /* 搬砖 */
.MLGB {
    height: 500px;
    background-color: antiquewhite;
}
.header {
    height: 50px;
    line-height: 50px;
    font-size: 18px;
    color: #fff;
    text-align: center;
    background-color: #f97c7c;
}
.nav {
    height: 100px;
}
.box {
    display: block;
    width: 100%;
    max-width:187px;
    float: left;
    height: 100px;
    line-height: 100px;
    text-align: center;
    text-decoration: none;
    font-size: 18px;
    border: 1px solid #ddd;
}
```    
![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/14.png)

你陷入了沉思，经过短短3个小时的深思熟虑，将CSS改成如上。
你发现，入口虽然排版变好看了，但是，入口元素高度却超出板砖盒子范围了，而且，nav的高度也是固定的。
于是，你动手优化了起来。

```css
 /* 搬砖 */
.MLGB {
    /* height: 500px; */
    background-color: antiquewhite;
}
.header {
    height: 50px;
    line-height: 50px;
    font-size: 18px;
    color: #fff;
    text-align: center;
    background-color: #f97c7c;
}
.nav {
    /* height: 100px; */
}
.nav::after{
    content:"";
    display: block;
    height: 0;
    clear: both;
    overflow: hidden;
}
.box {
    display: block;
    width: 100%;
    max-width: 187px;
    float: left;
    height: 100px;
    line-height: 100px;
    text-align: center;
    text-decoration: none;
    font-size: 18px;
    border: 1px solid #ddd;
}
```

![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/15.png)

但是，你很快发现，测试又来了。
你有点怀疑，她是不是喜欢你？但是，手机上的测试效果，让你暂时打消了这怀疑。

![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/16.png)

没错，她的是iphone5，而你的是iphone6。
你很快发现了，那个box的宽度不能写死。
弥留，哦，不，迷茫之际，你想起了昨天仔细研究过的《高级前端必会的flex布局》。

```css
 /* 重置一下 */
* {
    padding: 0;
    border: 0;
    margin: 0;
    outline: 0;
    box-sizing: border-box;
}
 /* 搬砖 */
.MLGB {
    /* height: 500px; */
    background-color: antiquewhite;
}
.header {
    height: 50px;
    line-height: 50px;
    font-size: 18px;
    color: #fff;
    text-align: center;
    background-color: #f97c7c;
}
.nav {
    /* height: 100px; */
    display: flex;
    flex-wrap: wrap;
}
.nav::after {
    content: "";
    display: block;
    height: 0;
    clear: both;
    overflow: hidden;
}
.box {
    display: flex;
    justify-content: center;
    flex: 1 1 auto;
    min-width: 160px;
    height: 100px;
    line-height: 100px;
    text-decoration: none;
    font-size: 18px;
    border: 1px solid #ddd;
}
```
![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/17.png)

你的iphone6

![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/18.png)

她的iphone5
你发现，你的iphone6，她的iphone5都正常了。

## 同时，更复杂的需求又来了

领导说，要做一个，用户购物车，收藏，设置，查看过的商品侧边栏，类似QQ那样。PC端默认显示，手机端默认隐藏，而且在头部区域，显示一个能够点击弹出侧边栏的按钮。
```css
 /* 重置一下 */
* {
    padding: 0;
    border: 0;
    margin: 0;
    outline: 0;
    box-sizing: border-box;
}
 /* 搬砖 */
.MLGB {
    /* height: 500px; */
    background-color: antiquewhite;
}
.header {
    height: 50px;
    line-height: 50px;
    font-size: 18px;
    color: #fff;
    text-align: center;
    background-color: #f97c7c;
}
.nav {
    /* height: 100px; */
    display: flex;
    flex-wrap: wrap;
}
.nav::after {
    content: "";
    display: block;
    height: 0;
    clear: both;
    overflow: hidden;
}
.box {
    display: flex;
    justify-content: center;
    flex: 1 1 auto;
    min-width: 160px;
    height: 100px;
    line-height: 100px;
    text-decoration: none;
    font-size: 18px;
    border: 1px solid #ddd;
}
```
```html
<div class="MLGB">
    <!-- 头部 -->
    <div class="header">
        欢迎大家来到，双十一天猫主会场！
    </div>
    <!-- 主要内容区域 -->
    <div class="main">
        <!-- 左侧菜单 -->
        <div class="menu">
            <div class="li">购物车</div>
            <div class="li">我的收藏</div>
            <div class="li">浏览记录</div>
            <div class="li">已经购买</div>
            <div class="li">设置</div>
            <div class="li">退出</div>
        </div>
        <!-- 分会场入口 -->
        <div class="nav">
            <a class="box" href="##">鞋子</a>
            <a class="box" href="##">箱包</a>
            <a class="box" href="##">数码</a>
            <a class="box" href="##">服装</a>
            <a class="box" href="##">乐器</a>
            <a class="box" href="##">户外</a>
            <a class="box" href="##">家具</a>
            <a class="box" href="##">家具</a>
            <a class="box" href="##">影视</a>
            <a class="box" href="##">美食</a>
        </div>
    </div>
</div>
```
![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/19.png)

很快，PC端的效果就实现了。
令人头疼的移动端该怎么做呢？
万能的js大人肯定是有办法解决的，但是，杀鸡焉用牛刀，难道就没有更简单的方法吗？

![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/20.png)

伟大的CSS大人，从来不会让我们高级前端难堪。
它传之于世的《CSS圣经》中，早已准备好了一切。
果然，乱军从中，被你找到了蛛丝马迹。
媒体查询（@media），这个专为响应式而生的时势英雄，终于要从尘封的历史遗迹中走出来了。
```css
/* 重置一下 */
* {
    padding: 0;
    border: 0;
    margin: 0;
    outline: 0;
    box-sizing: border-box;
}
 /* 搬砖 */
.MLGB {
    /* height: 500px; */
    background-color: antiquewhite;
}
.header {
    display: flex;
    align-items: center;
    height: 50px;
    font-size: 18px;
    padding: 0 10px;
    color: #fff;
    text-align: center;
    background-color: #f97c7c;
}
.main {
    display: flex;
}
/* 切换菜单的按钮 */
.toggle-menu {
    height: 30px;
    line-height: 30px;
    text-align: center;
    width: 30px;
    font-size: 14px;
    background-color: #607d8b;
    margin-right: 10px;
}
/* 菜单 */
.menu {
    flex: 0 0 140px;
    background-color: #5ed5e4;
}
.menu .li {
    height: 30px;
    line-height: 30px;
    padding: 0 10px;
    border-bottom: 1px solid #91dfe8;
}
.nav {
    /* height: 100px; */
    display: flex;
    flex-wrap: wrap;
    flex: 1 1 100%;
}
.nav::after {
    content: "";
    display: block;
    height: 0;
    clear: both;
    overflow: hidden;
}
.box {
    display: flex;
    justify-content: center;
    flex: 1 1 auto;
    min-width: 160px;
    height: 100px;
    line-height: 100px;
    text-decoration: none;
    font-size: 18px;
    border: 1px solid #ddd;
}
```
```html
<div class="MLGB">
    <!-- 头部 -->
    <div class="header">
        <div class="toggle-menu">菜</div>
        <div class="title">欢迎大家来到，双十一天猫主会场！</div>
    </div>
    <!-- 主要内容区域 -->
    <div class="main">
        <!-- 左侧菜单 -->
        <div class="menu">
            <div class="li">购物车</div>
            <div class="li">我的收藏</div>
            <div class="li">浏览记录</div>
            <div class="li">已经购买</div>
            <div class="li">设置</div>
            <div class="li">退出</div>
        </div>
        <!-- 分会场入口 -->
        <div class="nav">
            <a class="box" href="##">鞋子</a>
            <a class="box" href="##">箱包</a>
            <a class="box" href="##">数码</a>
            <a class="box" href="##">服装</a>
            <a class="box" href="##">乐器</a>
            <a class="box" href="##">户外</a>
            <a class="box" href="##">家具</a>
            <a class="box" href="##">家具</a>
            <a class="box" href="##">影视</a>
            <a class="box" href="##">美食</a>
        </div>
    </div>
</div>
```

![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/21.png)

首先呢，你没有管其他乱起八遭的东西，先简单粗暴地让这个菜单显示出来。
因为，作为一个拥有高级思维的高级前端，你知道，想那么多是没用的。
接下来你要干嘛呢？你要把这个菜单，隐藏起来，因为目前是PC端。


```css
@media screen and (min-width: 500px) {
    .header .toggle-menu {
        display: none;
    }
}
```
![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/22.png)

十分完美，@media果然厉害。
再接下来要干嘛呢？
移动端按钮显示，菜单隐藏。

```css
 /* PC端要做的 */
@media screen and (min-width: 500px) {
    .header .toggle-menu {
        display: none;
    }
}

/* 移动端要做的 */
@media screen and (max-width: 500px) {
    .header .toggle-menu {
        display: block;
    }
    .menu {
        display: none;
    }
}
```

![img](https://banshiweichen.gitee.io/chensuiyi-static-server/suiyi-1/23.png)

看起来十分完美，不用费javascript一兵一卒就搞定了。
更何况，这个方法，比写一堆js优雅多了。
接下来要干嘛呢？给按钮绑定点击事件，点击切换菜单的display值就行了。
那么，这里呢，就暂且不表。
由于时间关系呢，站长还有很多事做，坚持每天写一篇对于目前来说，已经有点难度了。
也是因为时间的关系，本文并没有更加详细地讲述关于响应式的方方面面和各种解决方法，各种坑。
不过，也足以抛砖引玉，解决同学们的一部分关于响应式的疑惑。
记住那个妙言：响应不同屏幕设备合适地展现网页效果的方式或着手段。
响应式是一种解决不同屏幕正确且合适地显示网页内容的思想和方法，它并不等于框架，更不等于bootstrap。
知其然，知其所以然。

何以解忧，唯有编程，我是，让天下没有难学的编程。
微信（c91374286）


 
