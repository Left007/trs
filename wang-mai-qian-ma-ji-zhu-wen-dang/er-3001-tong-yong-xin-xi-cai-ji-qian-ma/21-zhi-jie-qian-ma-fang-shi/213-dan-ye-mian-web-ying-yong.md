### 2.1.3 单页面Web应用

如果站点是基于Angular.js、Vue.js等构建的单页面应用，页面嵌码也有调整。由于单页面应用就只有一个页面，浏览器一开始会加载必须的HTML、CSS、JavaScript，之后的操作都是在这个页面上的。如果嵌码采用普通的方式，那么不管在站点内如何切换页面，PV只有一个。

所以，为了实现在切换路由时可以实现PV的获取，有两个要求：

* 站点需要以hash的方式作为路由模式
* 需要在上面获取代码的后面增加标记“&siteType=spa”，以开启hash改变时发送PV

```
<script id="_trs_ta_js" src="//ta.8531.cn/c/js/ta.js?mpid=204&siteType=spa " async="async" defer="defer"></script>
```


