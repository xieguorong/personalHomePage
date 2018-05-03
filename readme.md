一个建设中的个人网站
====

[主页](http://htmlpreview.github.io/?https://github.com/BUPTlhuanyu/personalHomePage/blob/master/src/index.html)

####
    打算写两个版本，原生js版本以及vue版本或者react版本
    原生js版本主要存在的问题有
+   异步管理，将使用定时器，事件处理程序，以及es6的promise，generator，async管理异步流程
+   数据的双向绑定
+   原生js的路由管理
+   CSS文件的划分，布局，效果等等分离文件，主要利于开发
+   js文件，申明文件以及调用文件分离
    性能优化
+   webpack抽取文件，合并js文件与css文件，加快线上网站的加载速度
+   背景图片，等图片的优化：利用tinypng在线工具对图片进行无损压缩。
+   数据的分组处理，由于浏览器单线程具有阻塞性，避免js处理获取的数据时间过长，阻塞页面用户的交互。
        并发协作：将一个长期运行的代码（“进程”）分割为多个步骤或者所多批任务，使得其他并发“进程”有机会将自己的运算插入到事件循环队列中交替运行。
        长期运行的“进程”运行时，页面上的其他代码都不能运行，包括不能有其他的 response(..)调用或 UI 刷新，甚至是像滚动、输入、按钮点击这样的用户事件。
        所以，要创建一个协作性更强更友好且不会霸占事件循环队列的并发系统，你可以异步地批处理这些结果。每次处理之后返回事件循环，让其他等待事件有机会运行。
        可以利用steTimeout(...,0)来实现。参考《js高级程序设计》第22章YieldingProcesses或者《你不知道的JS中》1.4.3协作
        另外：强力推荐一篇详解[事件循环和任务队列](https://www.jianshu.com/p/4516ad4b3048)的文章
+   对DOM执行集中添加操作
+   减少http请求
+   ajax缓存


#####   CSS
+   两列流式布局，三列流式布局，混合流式布局。未使用flex
+   清除浮动方法的比较，主要用了常用的clearfix的布局
+   浮动定位
+   页脚始终保持在html底部，min-height
+   水平垂直居中

#####   js
+   利用豆瓣API，生成电影榜单:利用jsonp跨域，解决chrome等浏览器的阻止混合内容，取消逐个添加DOM，解决响应完成的一些异步问题。
+   利用qq音乐API，为音乐播放器提供资源

![图片](main.png)
![图片](life.png)