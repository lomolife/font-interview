# font-interview
##前端面试问题总结&笔记（总结自网络部分来源自己）
#### 开放性题目

        1.自我介绍
        2.项目介绍
        3.各种前端方面的问题
        4.怎么学前端的
        

#### 美团电面总结：

      1.项目架构

      2.怎么绑定一个点击事件
      
      3.em和rem的区别
      
     'em' :em是相对单位，em的基准点是与其父节点相关
     'rem' : rem也是相对单位，但是rem的基准点是与根节点相关
     ...

#### 大众点评电面总结:

      1.一个width：100%的div里套两个div，一个div，width:100px;怎样使另一个div填充后面的内容
    - 简单至极：给第二个div加一个height就可以了
      2.position的值， relative和absolute分别是相对于谁进行定位的？

      - `absolute` :生成绝对定位的元素， 相对于最近一级的 定位不是 static 的父元素来进行定位。

      - `fixed` :（老IE不支持）生成绝对定位的元素，通常相对于浏览器窗口或 frame 进行定位。

      - `relative` :生成相对定位的元素，相对于其在普通流中的位置进行定位。

      - `static`  :默认值。没有定位，元素出现在正常的流中

      - `sticky` :生成粘性定位的元素，容器的位置根据正常文档流计算得出
      ...

#### 创建ajax过程：

      1.创建XMLHttpRequest对象,也就是创建一个异步调用对象.
      2.创建一个新的HTTP请求,并指定该HTTP请求的方法、URL及验证信息.
      3.设置响应HTTP请求状态变化的函数.
      4.发送HTTP请求.
      5.获取异步调用返回的数据.
      6.使用JavaScript和DOM实现局部刷新.
      
#### DOCTYPE

      DOCTYPE(Document Type),该声明位于文档中最前面的位置,处于html标签之前,此标签告知浏览器文档使用哪种HTML或者XHTML规范.


#### SEO优化

      1.页面描述
      每个网页都应有一个不超过 150 个字符且能准确反映网页内容的描述标签
      <meta name="description" content="不超过150个字符"> <!-- 页面描述 -->
      
      2.页面关键词
      <meta name="keywords" content=""> <!-- 页面关键词 -->
      
      3.定义网页搜索引擎索引方式,robotterms是一组使用英文逗号「,」分割的值,通常有如下几种取值：
      none，noindex，nofollow，all，index和follow
      <meta name="robots" content="index,follow"> <!-- 搜索引擎抓取 -->
      
      
      
      
      

####移动端的头部标签和meta
```html
<!DOCTYPE html> <!-- 使用 HTML5 doctype，不区分大小写 -->
<html lang="zh-cmn-Hans"> <!-- 更加标准的 lang 属性写法 http://zhi.hu/XyIa -->
<head>
    <!-- 声明文档使用的字符编码 -->
    <meta charset='utf-8'>
    <!-- 优先使用 IE 最新版本和 Chrome -->
    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1"/>
    <!-- 页面描述 -->
    <meta name="description" content="不超过150个字符"/>
    <!-- 页面关键词 -->
    <meta name="keywords" content=""/>
    <!-- 网页作者 -->
    <meta name="author" content="name, email@gmail.com"/>
    <!-- 搜索引擎抓取 -->
    <meta name="robots" content="index,follow"/>
    <!-- 为移动设备添加 viewport -->
    <meta name="viewport" content="initial-scale=1, maximum-scale=3, minimum-scale=1, user-scalable=no">
    <!-- `width=device-width` 会导致 iPhone 5 添加到主屏后以 WebApp 全屏模式打开页面时出现黑边 http://bigc.at/ios-webapp-viewport-meta.orz -->
 
    <!-- iOS 设备 begin -->
    <meta name="apple-mobile-web-app-title" content="标题">
    <!-- 添加到主屏后的标题（iOS 6 新增） -->
    <meta name="apple-mobile-web-app-capable" content="yes"/>
    <!-- 是否启用 WebApp 全屏模式，删除苹果默认的工具栏和菜单栏 -->
 
    <meta name="apple-itunes-app" content="app-id=myAppStoreID, affiliate-data=myAffiliateData, app-argument=myURL">
    <!-- 添加智能 App 广告条 Smart App Banner（iOS 6+ Safari） -->
    <meta name="apple-mobile-web-app-status-bar-style" content="black"/>
    <!-- 设置苹果工具栏颜色 -->
    <meta name="format-detection" content="telphone=no, email=no"/>
    <!-- 忽略页面中的数字识别为电话，忽略email识别 -->
    <!-- 启用360浏览器的极速模式(webkit) -->
    <meta name="renderer" content="webkit">
    <!-- 避免IE使用兼容模式 -->
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <!-- 针对手持设备优化，主要是针对一些老的不识别viewport的浏览器，比如黑莓 -->
    <meta name="HandheldFriendly" content="true">
    <!-- 微软的老式浏览器 -->
    <meta name="MobileOptimized" content="320">
    <!-- uc强制竖屏 -->
    <meta name="screen-orientation" content="portrait">
    <!-- QQ强制竖屏 -->
    <meta name="x5-orientation" content="portrait">
    <!-- UC强制全屏 -->
    <meta name="full-screen" content="yes">
    <!-- QQ强制全屏 -->
    <meta name="x5-fullscreen" content="true">
    <!-- UC应用模式 -->
    <meta name="browsermode" content="application">
    <!-- QQ应用模式 -->
    <meta name="x5-page-mode" content="app">
    <!-- windows phone 点击无高光 -->
    <meta name="msapplication-tap-highlight" content="no">
    <!-- iOS 图标 begin -->
    <link rel="apple-touch-icon-precomposed" href="/apple-touch-icon-57x57-precomposed.png"/>
    <!-- iPhone 和 iTouch，默认 57x57 像素，必须有 -->
    <link rel="apple-touch-icon-precomposed" sizes="114x114" href="/apple-touch-icon-114x114-precomposed.png"/>
    <!-- Retina iPhone 和 Retina iTouch，114x114 像素，可以没有，但推荐有 -->
    <link rel="apple-touch-icon-precomposed" sizes="144x144" href="/apple-touch-icon-144x144-precomposed.png"/>
    <!-- Retina iPad，144x144 像素，可以没有，但推荐有 -->
    <!-- iOS 图标 end -->
 
    <!-- iOS 启动画面 begin -->
    <link rel="apple-touch-startup-image" sizes="768x1004" href="/splash-screen-768x1004.png"/>
    <!-- iPad 竖屏 768 x 1004（标准分辨率） -->
    <link rel="apple-touch-startup-image" sizes="1536x2008" href="/splash-screen-1536x2008.png"/>
    <!-- iPad 竖屏 1536x2008（Retina） -->
    <link rel="apple-touch-startup-image" sizes="1024x748" href="/Default-Portrait-1024x748.png"/>
    <!-- iPad 横屏 1024x748（标准分辨率） -->
    <link rel="apple-touch-startup-image" sizes="2048x1496" href="/splash-screen-2048x1496.png"/>
    <!-- iPad 横屏 2048x1496（Retina） -->
 
    <link rel="apple-touch-startup-image" href="/splash-screen-320x480.png"/>
    <!-- iPhone/iPod Touch 竖屏 320x480 (标准分辨率) -->
    <link rel="apple-touch-startup-image" sizes="640x960" href="/splash-screen-640x960.png"/>
    <!-- iPhone/iPod Touch 竖屏 640x960 (Retina) -->
    <link rel="apple-touch-startup-image" sizes="640x1136" href="/splash-screen-640x1136.png"/>
    <!-- iPhone 5/iPod Touch 5 竖屏 640x1136 (Retina) -->
    <!-- iOS 启动画面 end -->
 
    <!-- iOS 设备 end -->
    <meta name="msapplication-TileColor" content="#000"/>
    <!-- Windows 8 磁贴颜色 -->
    <meta name="msapplication-TileImage" content="icon.png"/>
    <!-- Windows 8 磁贴图标 -->
 
    <link rel="alternate" type="application/rss+xml" title="RSS" href="/rss.xml"/>
    <!-- 添加 RSS 订阅 -->
    <link rel="shortcut icon" type="image/ico" href="/favicon.ico"/>
    <!-- 添加 favicon icon -->
 
    <title>标题</title>
</head>
```

#### 解释下浮动和它的工作原理？清除浮动的技巧
     
     浮动元素脱离文档流，不占据空间。浮动元素碰到包含它的边框或者浮动元素的边框停留。
     
     1.使用空标签清除浮动。
     
     这种方法是在所有浮动标签后面添加一个空标签 定义css clear:both. 弊端就是增加了无意义标签。

     2.使用overflow。

     给包含浮动元素的父标签添加css属性 overflow:auto; zoom:1; zoom:1用于兼容IE6。

     3.使用after伪对象清除浮动。

     该方法只适用于非IE浏览器。具体写法可参照以下示例。使用中需注意以下几点。一、该方法中必须为需要清除浮动元素的伪对象中设置 height:0，否则该元素会比实际高出若干像素；

#### 浮动元素引起的问题和解决办法？

     浮动元素引起的问题：

    （1）父元素的高度无法被撑开，影响与父元素同级的元素

    （2）与浮动元素同级的非浮动元素（内联元素）会跟随其后

    （3）若非第一个元素浮动，则该元素之前的元素也需要浮动，否则会影响页面显示的结构
    
& 解决办法

使用CSS中的clear:both;属性来清除元素的浮动可解决2、3问题，对于问题1，添加如下样式，给父元素添加clearfix样式：

```css
.clearfix:after{content: ".";display: block;height: 0;clear: both;visibility: hidden;}

    .clearfix{display: inline-block;} /* for IE/Mac */
```

#### 清除浮动的几种方法：

        1，额外标签法，<div style="clear:both;"></div>（缺点：不过这个办法会增加额外的标签使HTML结构看起来不够简洁。）

        2，使用after伪类

         #parent:after{

         content:".";

         height:0;

         visibility:hidden;

         display:block;

         clear:both;

         }


       3,浮动外部元素

       4,设置overflow为hidden或者auto

#### html5有哪些新特性、移除了那些元素？如何处理HTML5新标签的浏览器兼容问题？如何区分 HTML 和 HTML5？

    HTML5 现在已经不是 SGML 的子集，主要是关于图像，位置，存储，多任务等功能的增加。

    拖拽释放(Drag and drop) API

    语义化更好的内容标签（header,nav,footer,aside,article,section）

    音频、视频API(audio,video)

    画布(Canvas) API

    地理(Geolocation) API

    本地离线存储 localStorage 长期存储数据，浏览器关闭后数据不丢失；

    sessionStorage 的数据在浏览器关闭后自动删除


    表单控件，calendar、date、time、email、url、search

    新的技术webworker, websocket, GeolocationHTML5 现在已经不是 SGML 的子集，主要是关于图像，位置，存储，多任务等功能的增加。

    拖拽释放(Drag and drop) API

    语义化更好的内容标签（header,nav,footer,aside,article,section）

    音频、视频API(audio,video)

    画布(Canvas) API

    地理(Geolocation) API

    本地离线存储 localStorage 长期存储数据，浏览器关闭后数据不丢失；

    sessionStorage 的数据在浏览器关闭后自动删除

    表单控件，calendar、date、time、email、url、search

    新的技术webworker, websocket, Geolocation
  
    &移除的元素
  
    纯表现的元素：basefont，big，center，font, s，strike，tt，u；

    对可用性产生负面影响的元素：frame，frameset，noframes；
  
    &支持HTML5新标签：
  
     IE8/IE7/IE6支持通过document.createElement方法产生的标签，

     可以利用这一特性让这些浏览器支持HTML5新标签，

     当然最好的方式是直接使用成熟的框架、使用最多的是html5shim框架

```html
       <!--[if lt IE 9]>

       <script> src="http://html5shim.googlecode.com/svn/trunk/html5.js"</script>

       <![endif]-->
```
    如何区分： DOCTYPE声明\新增的结构元素\功能元素


#### 说说你对MVC和MVVM的理解

>`MVC`
    
    View 传送指令到 Controller
    
    Controller 完成业务逻辑后，要求 Model 改变状态
    
    Model 将新的数据发送到 View，用户得到反馈
    
    
所有通信都是单向的。

`Angular`它采用双向绑定（data-binding）：`View`的变动，自动反映在 `ViewModel`，反之亦然。


    组成部分Model、View、ViewModel

    View：UI界面

    ViewModel：它是View的抽象，负责View与Model之间信息转换，将View的Command传送到Model；

    Model：数据访问层
    
#### 校招笔试总结

> 字符串反置

```html
        <script>
        var str = "www.123.com",
        result = "";
        for(var i = str.length; i > 0; i--) {
        result += str.charAt(i - 1);
        }
        console.log(result);//结果为"moc.321.www"
        </script>
```
