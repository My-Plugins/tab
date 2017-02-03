### 封装tab栏切换使用说明
1.tab.js是采用面向对象的方式进行封装实现代码功能的。
2.引入css文件
```js
<link rel="stylesheet" type="text/css" href="css/tab.css">
```
3.html代码
```js
<div class="wrapper" id="wrapper">
        <ul class="tab" id="tab-menu">
            <li class="tab-item active">国际大牌<span>◆</span></li>
            <li class="tab-item">国妆名牌<span>◆</span></li>
            <li class="tab-item">清洁用品<span>◆</span></li>
            <li class="tab-item">男士精品</li>
        </ul>
        <div class="products" id="tab-main">
            <div class="main selected">
                <a href="###"><img src="imgs/guojidapai.jpg" alt=""/></a>
            </div>
            <div class="main">
                <a href="###"><img src="imgs/guozhuangmingpin.jpg" alt=""/></a>
            </div>
            <div class="main">
                <a href="###"><img src="imgs/qingjieyongpin.jpg" alt=""/></a>
            </div>
            <div class="main">
                <a href="###"><img src="imgs/nanshijingpin.jpg" alt=""/></a>
            </div>
        </div>
    </div>
```
3.引入tab.js包
```js
<script type="text/javascript" src="js/tab.js"></script>
```

4.开始使用tab.js
```js
  new Tab({
        tabMenu: "tab-menu",   // 指定tab栏菜单的id
        tabMain: "tab-main",   // 指定tab栏内容区域的id
        auto: true,               // 指定是否自动播放
        tempStep: 1500            // 指定时间间隔
      })
```
5.效果图：![](https://raw.githubusercontent.com/Believel/MarkdownPhotos/master/imgs/tab.png)
