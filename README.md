# font-interview
##前端面试问题总结（总结自网络部分来源自己）
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
      

