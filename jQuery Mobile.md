# jQuery Mobile
1. jQuery Mobile 是创建移动 web 应用程序的框架。
2. jQuery Mobile 适用于所有流行的智能手机和平板电脑。
3. jQuery Mobile 使用 HTML5 和 CSS3 通过尽可能少的脚本对页面进行布局。
## 下载安装
1. 从 CDN 引用 jQuery Mobile（推荐）
2. CDN (Content Delivery Network) 用于通过 web 来分发常用的文件，以此加快用户的下载速度。
3. 与 jQuery 类似，无需在您的计算机上安装任何程序；您只需直接在 HTML 页面中引用以下样式表和 JavaScript 库，这样 jQuery Mobile 就可以工作了

```
<link href="https://cdn.bootcss.com/jquery-mobile/1.4.5/jquery.mobile.min.css" rel="stylesheet">
<script src="https://cdn.bootcss.com/jquery/1.12.4/jquery.min.js"></script>
<script src="https://cdn.bootcss.com/jquery-mobile/1.4.5/jquery.mobile.min.js"></script>
```

  
  [jQuery-Mobile的CDN](http://www.bootcdn.cn/jquery-mobile/)
  
  [jQueryCDN](http://www.bootcdn.cn/jquery/)
  
2. 从 jQuerymobile.com 下载 jQuery Mobile 库

## jQuery Mobile 页面
```
<body>
   <div data-role="page">

      <div data-role="header">
           <h1>欢迎访问我的主页</h1>
      </div>

      <div data-role="content">
          <p>我是一名移动开发者！</p>
      </div>

      <div data-role="footer">
          <h1>页脚文本</h1>
      </div>

   </div>
</body>
```

1. data-role="page" 是显示在浏览器中的页面
2. data-role="header" 创建页面上方的工具栏（常用于标题和搜索按钮）
3. data-role="content" 定义页面的内容，比如文本、图像、表单和按钮，等等
4. data-role="footer" 创建页面底部的工具栏

### 在 jQuery Mobile 中创建按钮
#### jQuery Mobile 中的按钮可通过三种方法创建：
1. 使用 < button > 元素
2. 使用 < input > 元素
3. 使用 data-role="button" 的 <a> 元素

**jQuery Mobile 中的按钮会自动获得样式，这增强了他们在移动设备上的交互性和可用性。**
**data-role="button" 的 <a> 元素来创建页面之间的链接，而 <input> 或 <button> 元素用于表单提交。**
  
 ### 行内按钮
默认情况下，按钮会占据屏幕的全部宽度。如果您需要按钮适应其内容，或者如果您需要两个或多个按钮并排显示，请添加 data-inline="true"
```
<a href="#pagetwo" data-role="button" data-inline="true">转到页面二</a>
```
### 组合按钮
jQuery Mobile 提供了对按钮进行组合的简单方法。
请将 data-role="controlgroup" 属性与 data-type="horizontal|vertical" 一同使用，以规定水平或垂直地组合按钮
```
<div data-role="controlgroup" data-type="horizontal">
  <a href="#anylink" data-role="button">按钮 1</a>
  <a href="#anylink" data-role="button">按钮 2</a>
  <a href="#anylink" data-role="button">按钮 3</a>
</div>`
```
### 后退按钮
```
<button  data-rel="back">按钮</button>
```

  


