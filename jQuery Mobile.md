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
### 更多用于按钮的 data-* 属性

属性| 值 | 描述|
-----|------|-----
data-corners	| true | false| 规定按钮是否有圆角。
data-mini| true | false| 规定是否是小型按钮。
data-shadow|true | false|规定按钮是否有阴影

```
<a href="#" data-role="button" data-inline="true" data-corners="true" data-mini="true" data-shadow="true">按钮 1</a>
<a href="#" data-role="button" data-inline="true" data-corners="false" data-mini="false" data-shadow="false">按钮 1</a>
```
### jQuery Mobile 按钮图标
1. jQuery Mobile 提供的一套图标可令您的按钮更具吸引力
2.如需在 jQuery Mobile 中向按钮添加图标，请使用 data-icon 属性：
**您也可以在 <button> 或 <input> 元素中使用 data-icon 属性。**

```
<a href="#anylink" data-role="button" data-icon="refresh">Refresh Page</a>
```

属性| 值 | 描述|
-----|------|-----
data-icon="arrow-l"	| 左箭头| 
data-icon="arrow-r" | 右箭头	|	
data-icon="arrow-u"	|上箭头	|	
data-icon="arrow-d" |	下箭头	|	
data-icon="plus"	  |加		|
data-icon="minus"	  |减		|
data-icon="delete"	|删除		|
data-icon="check"	  |检查		|
data-icon="home"	  |首页		|
data-icon="info"	  |信息		|
data-icon="grid"    |网格		|
data-icon="gear"	  |齿轮		|
data-icon="search"	|搜索		|
data-icon="back"	  |后退		|
data-icon="forward"	|向前		|
data-icon="refresh" |刷新		|
data-icon="star"	  |星		|
data-icon="alert"	  |提醒  |

```
	<a href="index.html" data-role="button" data-icon="bars" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="edit" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="arrow-l" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="arrow-r" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="arrow-u" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="arrow-d" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="delete" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="plus" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="minus" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="check" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
    <a href="index.html" data-role="button" data-icon="gear" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="refresh" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="forward" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="back" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="grid" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="star" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="alert" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="info" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="home" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
		<a href="index.html" data-role="button" data-icon="search" data-iconpos="notext" data-theme="a" data-inline="true">My button</a>
```

### 定位图标
1. 您也能够规定图标被放置的位置：上、右、下或左。
2. 请使用 data-iconpos 属性来规定位置
3. 默认地，所有按钮中的图标靠左放置。
```
<a href="#link" data-role="button" data-icon="search" data-iconpos="top">上</a>
<a href="#link" data-role="button" data-icon="search" data-iconpos="right">右</a>
<a href="#link" data-role="button" data-icon="search" data-iconpos="bottom">下</a>
<a href="#link" data-role="button" data-icon="search" data-iconpos="left">左</a>

```
### 只显示图标
1. 如果只需显示图标，请将 data-iconpos 设置为 "notext"
```
<a href="#link" data-role="button" data-icon="search" data-iconpos="notext">搜索</a>
```











  


