# HTML语言：

### 标题：
```
标题（Heading）是通过 <h1> - <h6> 等标签进行定义的，<h1> 定义最大的标题，<h6> 定义最小的标题。
<hr /> 标签在 HTML 页面中创建水平线。
```

### 段落：
```
段落是通过 <p> 标签定义的。
<br /> 元素是一个空的 HTML 元素，一般用于换行或另起一行。
```

### 样式：
```
style 属性的作用：提供了一种改变所有 HTML 元素的样式的通用方法。
background-color 属性为元素定义了背景颜色。
font-family、color 以及 font-size 属性分别定义元素中文本的字体系列、颜色和字体尺寸。
text-align 属性规定了元素中文本的水平对齐方式
```

### 格式化：
```
标签	       描述
<b>	      定义粗体文本。
<big>	      定义大号字。
<em>	      定义着重文字。
<i>	      定义斜体字。
<small>	      定义小号字。
<strong>      定义加重语气。
<sub>	      定义下标字。
<sup>	      定义上标字。
<ins>	      定义插入字。
<del>	      定义删除字。
```

### 引用：
```
<q> 元素定义短的引用，浏览器通常会为 <q> 元素包围引号。
<blockquote> 元素定义被引用的节，浏览器通常会对 <blockquote> 元素进行缩进处理。
<abbr> 元素定义缩写或首字母缩略语。
<dfn> 元素定义项目或缩写的定义。
<bdo>定义文本方向。
```

### 注释：
```
在开始标签中有一个惊叹号，但是结束标签中没有。<!-- ...... -->
```

### 链接：
```
我们通过使用 <a> 标签在 HTML 中创建链接。
有两种使用 <a> 标签的方式：
通过使用 href 属性 - 创建指向另一个文档的链接；
通过使用 name 属性 - 创建文档内的书签。
使用 Target 属性，你可以定义被链接的文档在何处显示。
```

### 图像：
```
图像由 <img> 标签定义，<img> 是空标签，意思是说，它只包含属性，并且没有闭合标签。
要在页面上显示图像，你需要使用源属性（src）。src 指 "source"。源属性的值是图像的 URL 地址。
alt 属性用来为图像定义一串预备的可替换的文本。替换文本属性的值是用户定义的。
```

###　表格：
```
每个表格由 <table> 标签开始。
每个表格行由 <tr> 标签开始。
每个表格数据由 <td> 标签开始。
表格的表头使用 <th> 标签进行定义。
(注：空的单元格的边框是不会被显示出来的。为了避免这种情况，在空单元格中添加一个空格占位符(&nbsp;)，就可以将边框显示出来。)
```

### 列表：
```
无序列表始于 <ul> 标签。每个列表项始于 <li>。
有序列表始于 <ol> 标签。每个列表项始于 <li> 标签。
自定义列表以 <dl> 标签开始。每个自定义列表项以 <dt> 开始。每个自定义列表项的定义以 <dd> 开始。
```

### 块，类，ID（用法：相当于先定义好头文件，再去调用头文件）：
```
HTML <div> 元素是块级元素，它是可用于组合其他 HTML 元素的容器，设置 <div> 元素的类，使我们能够为相同的 <div> 元素设置相同的类。
HTML <span> 元素是内联元素，可用作文本的容器，设置 <span> 元素的类，能够为相同的 <span> 元素设置相同的样式。
id 属性指定 HTML 元素的唯一 ID，id 的语法是：写一个井号 (#)，后跟一个 id 名称。然后，在花括号 {} 中定义 CSS 属性。
class 与 ID 的差异：同一个类名可以由多个 HTML 元素使用，而一个 id 名称只能由页面中的一个 HTML 元素使用。

<!DOCTYPE html>
<html>
<head>
<style>
/* 设置 id 为 "myHeader" 的元素的样式 */
#myHeader {
  background-color: lightblue;
  color: black;
  padding: 40px;
  text-align: center;
}

/* 设置类名为 "city" 的所有元素的样式 */
.city {
  background-color: tomato;
  color: white;
  padding: 10px;
} 
</style>
</head>
<body>

<h1>Class 与 ID 的差异</h1>

<p>一个类名可以由多个 HTML 元素使用，而一个 id 名称只能由页面中的一个 HTML 元素使用：</p>

<!-- 拥有唯一 id 的元素 -->
<h1 id="myHeader">我的城市</h1>

<!-- 拥有相同类名的多个元素 -->
<h2 class="city">上海</h2>
<p>中国最大的经济城市。</p>

<h2 class="city">深圳</h2>
<p>中国最具创新力的城市。</p>

<h2 class="city">北京</h2>
<p>中国的首都。</p>

</body>
</html>
```

### 内联框架：
```
iframe 的语法，<iframe src="URL"></iframe>。
height 和 width 属性用于规定 iframe 的高度和宽度。
frameborder 属性规定是否显示 iframe 周围的边框。
```

### JavaScript：
```
HTML <script> 标签用于定义客户端脚本（JavaScript）。
HTML <noscript> 标签定义了替代内容，这些内容将显示给在浏览器中禁用了脚本或浏览器不支持脚本的用户
```

### 文件路径：
```
绝对文件路径：绝对文件路径是指向一个因特网文件的完整 URL。
相对路径：相对路径指向了相对于当前页面的文件。
```

### 头部元素：
```
<head> 元素是所有头部元素的容器。<head> 内的元素可包含脚本，指示浏览器在何处可以找到样式表，提供元信息，等等。
<title> 标签定义文档的标题，title 元素在所有 HTML/XHTML 文档中都是必需的。用法：<title>...</title>
<base> 标签为页面上的所有链接规定默认地址或默认目标（target）。用法：<base ... />
<link> 标签定义文档与外部资源之间的关系，<link> 标签最常用于连接样式表。用法：<link ... />
<style> 标签用于为 HTML 文档定义样式信息，你可以在 style 元素内规定 HTML 元素在浏览器中呈现的样式。用法:<style>...</style>
<meta> 标签提供关于 HTML 文档的元数据。元数据不会显示在页面上，但是对于机器是可读的，典型的情况是，meta 元素被用于规定页面的描述、关键词、文档的作者、最后修改时间以及其他元数据，<meta> 标签始终位于 head 元素中，元数据可用于浏览器（如何显示内容或重新加载页面），搜索引擎（关键词），或其他 web 服务。用法：<meta ... />
```

### 布局：
```
<header>定义文档或节的页眉；
<nav>定义导航链接的容器；
<section>定义文档中的节；
<article>定义独立的自包含文章；
<aside>定义内容之外的内容（比如侧栏）；
<footer>定义文档或节的页脚；
<details>定义额外的细节；
<summary>定义 details 元素的标题。
（注：都可以在头文件先定义好，再在后面调用）
```

### 计算机代码元素：
```
<code>定义计算机代码文本。
<kbd>定义键盘文本。
<samp>定义计算机代码示例。
<var>定义变量。
<pre>定义预格式化文本。
```

### HTML5语义元素：
```
<article>定义文章。
<aside>定义页面内容以外的内容。
<details>定义用户能够查看或隐藏的额外细节。
<figcaption>定义 <figure> 元素的标题。
<figure>规定自包含内容，比如图示、图表、照片、代码清单等。
<footer>定义文档或节的页脚。
<header>规定文档或节的页眉。
<main>规定文档的主内容。
<mark>定义重要的或强调的文本。
<nav>定义导航链接。
<section>定义文档中的节。
<summary>定义 <details> 元素的可见标题。
<time>定义日期/时间。
```

### 字符实体：
```
显示结果	描述	                 实体名称	        实体编号
 	空格	                 &nbsp;	                &#160;
<	小于号	                 &lt;	                &#60;
>	大于号	                 &gt;	                &#62;
&	和号	                 &amp;	                &#38;
"	引号	                 &quot;	                &#34;
'	撇号 	                 &apos; (IE不支持)	&#39;
￠	分（cent）                &cent;	                &#162;
£	镑（pound）               &pound;	        &#163;
¥	元（yen）                 &yen;	                &#165;
€	欧元（euro）              &euro;	                &#8364;
§	小节	                 &sect;	                &#167;
©	版权（copyright）         &copy;	                &#169;
®	注册商标	                 &reg;	                &#174;
™	商标	                 &trade;	        &#8482;
×	乘号	                 &times;	        &#215;
÷	除号	                 &divide;	        &#247;
```

### 表情符号：
```
Emoji	值
🗻	&#128507;
🗼	&#128508;
🗽	&#128509;
🗾	&#128510;
🗿	&#128511;
😀	&#128512;
😁	&#128513;
😂	&#128514;
😃	&#128515;
😄	&#128516;
😅	&#128517;
```

### 字符集：
```
ASCII 字符集
ASCII 使用 0 到 31（以及 127）之间的值作为控制字符。
ASCII 使用 32 到 126 的值表示字母、数字和符号。
ASCII 不使用 128 到 255 之间的值。

ANSI 字符集 (Windows-1252)
对于 0 到 127 的值，ANSI 与 ASCII 相同。
ANSI 有一组专有的字符，其值从 128 到 159。
对于 160 到 255 的值，ANSI 与 UTF-8 相同。

ISO-8859-1 字符集
对于 0 到 127 的值，8859-1 与 ASCII 相同。
8859-1 不使用 128 到 159 之间的值。
对于从 160 到 255 的值，8859-1 与 UTF-8 相同。

UTF-8 字符集
对于 0 到 127 的值，UTF-8 与 ASCII 相同。
UTF-8 不使用 128到 159 之间的值。
对于 160 到 255 之间的值，UTF-8 与 ANSI 和 8859-1 相同。
UTF-8 从值 256 继续，包含超过 10000 个不同字符。
```

### 统一资源定位符（URL）：
```
语法规则：scheme://host.domain:port/path/filename

Scheme	       访问	                  用于...
http	       超文本传输协议	         以 http:// 开头的普通网页。不加密。
https	       安全超文本传输协议	         安全网页。加密所有信息交换。
ftp 	       文件传输协议	         用于将文件下载或上传至网站。
file	 	                         您计算机上的文件。

scheme - 定义因特网服务的类型。最常见的类型是 http；
host - 定义域主机（http 的默认主机是 www）；
domain - 定义因特网域名，比如 baidu.com；
:port - 定义主机上的端口号（http 的默认端口号是 80）；
path - 定义服务器上的路径（如果省略，则文档必须位于网站的根目录中）。
filename - 定义文档/资源的名称
```

### 框架：
```
框架结构标签（<frameset>）定义如何将窗口分割为框架，每个 frameset 定义了一系列行或列，rows/columns 的值规定了每行或每列占据屏幕的面积。
<Frame> 标签定义了放置在每个框架中的 HTML 文档。（注：如果不想用户通过拖动边框来改变它的大小可以在 <frame> 标签中加入属性：noresize="noresize"。）用法：<frame ... />
```

### 表单：
```
HTML 表单用于收集用户输入，<form> 元素定义 HTML 表单。

<input> 元素是最重要的表单元素，<input> 元素有很多形态，根据不同的 type 属性：（用法：<input ... />）
类型	描述
text	定义常规文本输入。
radio	定义单选按钮输入（选择多个选择之一）
submit	定义提交按钮（提交表单）
```

### 表单属性：
```
action 属性定义在提交表单时执行的动作，向服务器提交表单的通常做法是使用提交按钮，通常，表单会被提交到 web 服务器上的网页。（注：如果省略 action 属性，则将 action 设置为当前页面。）
method 属性规定在提交表单时所用的 HTTP 方法（GET 或 POST）。（注：默认值为 GET。）
Name 属性，如果要正确地被提交，每个输入字段必须设置一个 name 属性。
<fieldset> 元素组合表单中的相关数据，<legend> 元素为 <fieldset> 元素定义标题。
autocomplete 属性规定表单是否应打开自动完成功能，启用自动完成功能后，浏览器会根据用户之前输入的值自动填写值。
novalidate 属性是一个布尔属性，如果已设置，它规定提交时不应验证表单数据。

Form 中的 get 和 post 方法，在数据传输过程中分别对应了 HTTP 协议中的 GET 和 POST 方法。二者主要区别如下：
 1、Get 是用来从服务器上获得数据，而 Post 是用来向服务器上传递数据。
 2、Get 将表单中数据的按照 variable=value 的形式，添加到 action 所指向的 URL 后面，并且两者使用“?”连接，而各个变量之间使用“&”连接；Post 是将表单中的数据放在 form 的数据体中，按照变量和值相对应的方式，传递到 action 所指向 URL。
 3、Get 是不安全的，因为在传输过程，数据被放在请求的 URL 中，而如今现有的很多服务器、代理服务器或者用户代理都会将请求URL记录到日志文件中，然后放在某个地方，这样就可能会有一些隐私的信息被第三方看到。另外，用户也可以在浏览器上直接看到提交的数据，一些系统内部消息将会一同显示在用户面前。Post 的所有操作对用户来说都是不可见的。
 4、Get 传输的数据量小，这主要是因为受 URL 长度限制；而 Post 可以传输大量的数据，所以在上传文件只能使用 Post（当然还有一个原因，将在后面的提到）。
 5、Get 限制 Form 表单的数据集的值必须为 ASCII 字符；而 Post 支持整个 ISO10646 字符集。
 6、Get 是 Form 的默认方法。
(注：使用 Post 传输的数据，可以通过设置编码的方式正确转化中文；而 Get 传输的数据却没有变化。在以后的程序中，我们一定要注意这一点。）

Target 属性，target 属性规定提交表单后在何处显示响应。（注：默认值为 _self）
值	                描述
_blank	                响应显示在新窗口或选项卡中。
_self	                响应显示在当前窗口中。
_parent	                响应显示在父框架中。
_top	                响应显示在窗口的整个 body 中。
framename	        响应显示在命名的 iframe 中。
```

### 表单元素：
```
<select> 元素定义下拉列表。
<option> 元素定义待选择的选项，列表通常会把首个选项显示为被选选项，您能够通过添加 selected 属性来定义预定义选项。
<textarea> 元素定义多行输入字段（文本域）。
<button> 元素定义可点击的按钮。
<datalist> 元素为 <input> 元素规定预定义选项列表，用户会在他们输入数据时看到预定义选项的下拉列表，<input> 元素的 list 属性必须引用 <datalist> 元素的 id 属性。
```

### 输入类型：
```
text，<input type="text"> 定义供文本输入的单行输入字段。
password，<input type="password"> 定义密码字段。
submit，<input type="submit"> 定义提交表单数据至表单处理程序的按钮。
radio，<input type="radio"> 定义单选按钮。
checkbox，<input type="checkbox"> 定义复选框，复选框允许用户在有限数量的选项中选择零个或多个选项。
button，<input type="button> 定义按钮。
HTML5 增加了多个新的输入类型：
color；date；datetime；datetime-local；email；month；number；range；search；tel；time；url；week（注：老式 web 浏览器不支持的输入类型，会被视为输入类型 text。）
```

## 输入属性：
```
value 属性规定输入字段的初始值。
readonly 属性规定输入字段为只读（不能修改）。（注：readonly 属性不需要值。它等同于 readonly="readonly"。）
disabled 属性规定输入字段是禁用的，被禁用的元素是不可用和不可点击的，被禁用的元素不会被提交。（注：disabled 属性不需要值。它等同于 disabled="disabled"。）
size 属性规定输入字段的尺寸（以字符计）。
maxlength 属性规定输入字段允许的最大长度。
HTML5 为 <input> 增加了如下属性：
autocomplete；autofocus；form；formaction；formenctype；formmethod；formnovalidate；formtarget；height 和 width；list；min 和 max；multiple；pattern (regexp)；placeholder；required；step。并为 <form> 增加如需属性：autocomplete；novalidate。
```

### Input表单属性：
```
input 的 formaction 属性规定当提交表单时，对输入（数据）进行处理的文件的 URL，formaction 属性适用于以下输入类型：submit 和 image。（注：该属性会覆盖 <form> 元素的 action 属性）
input 的 formenctype 属性指定提交时应如何编码表单数据（仅适用于 method="post" 的表单），formenctype 属性适用于以下输入类型：submit 和 image。（注：此属性将覆盖 <form> 元素的 enctype 属性）
input 的 formmethod 属性定义了将表单数据发送到 action URL 的 HTTP 方法，formmethod 属性适用于以下输入类型：submit 和 image。（注：此属性将覆盖 <form> 元素的 method 属性。）
input 的 formtarget 属性指定一个名称或关键字，该名称或关键字规定在提交表单后在何处显示收到的响应，formtarget 属性适用于以下输入类型：submit 和 image。（注：此属性将覆盖 <form> 元素的 target 属性。）
input 的 formnovalidate 属性规定提交时不应验证 <input> 元素，formnovalidate 属性适用于以下输入类型：submit。（注：此属性将覆盖 <form> 元素的 novalidate 属性。）
```

### Canvas vs. SVG：
```
Canvas 和 SVG 都允许您在浏览器中创建图形，但是它们在根本上是不同的。
Canvas：依赖分辨率；不支持事件处理器；弱的文本渲染能力；能够以 .png 或 .jpg 格式保存结果图像；最适合图像密集型的游戏，其中的许多对象会被频繁重绘。
SVG：不依赖分辨率；支持事件处理器；最适合带有大型渲染区域的应用程序（比如谷歌地图）；复杂度高会减慢渲染速度（任何过度使用 DOM 的应用都不快）；不适合游戏应用。
```

### 插件、音频、视频：
```
<object> 元素：所有浏览器均支持 <object> 元素，<object> 元素定义 HTML 文档中的嵌入式对象。
<embed> 元素：这是一个 HTML5 标签，在 HTML4 中是非法的，但是所有主要浏览器均支持 <embed> 元素，<embed> 元素也可定义了 HTML 文档中的嵌入式对象。（注：<embed> 元素没有结束标记，它无法包含替代文本。）
<audio> 元素是一个 HTML5 元素，在 HTML 4 中是非法的，但在所有浏览器中都有效，<audio> 标签的作用是在 HTML 页面中嵌入音乐元素。
<video> 是 HTML 5 中的新标签，<video> 标签的作用是在 HTML 页面中嵌入视频元素。
<source>定义 <video> 和 <audio> 的来源。
<track>定义 <video> 和 <audio> 的轨道。
```

### HTML5 迁移：
```
修改文档类型：
从 HTML4 doctype：<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">修改为 HTML5 doctype：<!DOCTYPE html>
修改编码信息：
从 HTML4：<meta http-equiv="Content-Type" content="text/html;charset=utf-8">改为 HTML5：<meta charset="utf-8">
添加shiv：
<!--[if lt IE 9]>
  <script src="http://html5shiv.googlecode.com/svn/trunk/html5.js"></script>
<![endif]-->
更改为 HTML5 <header> 和 <footer>：
把 id="header" 和 id="footer" 的 <div> 元素修改为 HTML5 语义元素 <header> 和 <footer>
更改为 HTML5 <nav>：
把 id="menu" 的 <div> 元素修改为 HTML5 语义元素 <nav>
更改为 HTML5 <section>：
把 id="content" 的 the <div> 元素修改为 HTML5 语义元素 <section>
更改为 HTML5 <article>：
把 class="post" 的所有 <div> 元素修改为 HTML5 语义元素 <article>
```

### HTML5 拖放:
```
拖放（Drag 和 Drop）是很常见的特性。它指的是您抓取某物并拖入不同的位置。拖放是 HTML5 标准的组成部分：任何元素都是可拖放的。

<!DOCTYPE HTML>
<html>
<head>
<script>
function allowDrop(ev) {
    ev.preventDefault();
}
function drag(ev) {
    ev.dataTransfer.setData("text", ev.target.id);
}
function drop(ev) {
    ev.preventDefault();
    var data = ev.dataTransfer.getData("text");
    ev.target.appendChild(document.getElementById(data));
}
</script>
</head>
<body>
<div id="div1" ondrop="drop(event)" ondragover="allowDrop(event)"></div>
<img id="drag1" src="img_logo.gif" draggable="true" ondragstart="drag(event)" width="336" height="69">
</body>
</html>

把元素设置为可拖放
首先：为了把一个元素设置为可拖放，请把 draggable 属性设置为 true：
<img draggable="true">

拖放的内容 - ondragstart 和 setData()
然后，规定当元素被拖动时发生的事情。在上面的例子中， ondragstart 属性调用一个 drag(event) 函数，规定拖动什么数据。dataTransfer.setData() 方法设置被拖动数据的数据类型和值：
function drag(ev) {
    ev.dataTransfer.setData("text", ev.target.id);
}
在本例中，数据类型是 "text"，而值是这个可拖动元素的 id ("drag1")。

拖到何处 - ondragover
ondragover 事件规定被拖动的数据能够被放置到何处。默认地，数据/元素无法被放置到其他元素中。为了实现拖放，我们必须阻止元素的这种默认的处理方式。这个任务由 ondragover 事件的 event.preventDefault() 方法完成：
event.preventDefault()

进行放置 - ondrop
当放开被拖数据时，会发生 drop 事件。在上面的例子中，ondrop 属性调用了一个函数，drop(event)：
function drop(ev) {
    ev.preventDefault();
    var data = ev.dataTransfer.getData("text");
    ev.target.appendChild(document.getElementById(data));
}
代码解释：
调用 preventDefault() 来阻止数据的浏览器默认处理方式（drop 事件的默认行为是以链接形式打开）;
通过 dataTransfer.getData() 方法获得被拖的数据。该方法将返回在 setData() 方法中设置为相同类型的任何数据;
被拖数据是被拖元素的 id ("drag1");
把被拖元素追加到放置元素。
```

### HTML5 应用程序缓存：
```
使用应用程序缓存，通过创建 cache manifest 文件，可轻松创建 web 应用的离线版本。
HTML5 引入了应用程序缓存（Application Cache），这意味着可对 web 应用进行缓存，并可在没有因特网连接时进行访问。应用程序缓存为应用带来三个优势：
离线浏览 - 用户可在应用离线时使用它们
速度 - 已缓存资源加载得更快
减少服务器负载 - 浏览器将只从服务器下载更新过或更改过的资源

Cache Manifest 基础
如需启用应用程序缓存，请在文档的 <html> 标签中包含 manifest 属性：
<!DOCTYPE HTML>
<html manifest="demo.appcache">
...
</html>
每个指定了 manifest 的页面在用户对其访问时都会被缓存。如果未指定 manifest 属性，则页面不会被缓存（除非在 manifest 文件中直接指定了该页面）。manifest 文件的建议文件扩展名是：".appcache"。（注：manifest 文件需要设置正确的 MIME-type，即 "text/cache-manifest"。必须在 web 服务器上进行配置。）

Manifest 文件
manifest 文件是简单的文本文件，它告知浏览器被缓存的内容（以及不缓存的内容）。manifest 文件有三个部分：
CACHE MANIFEST - 在此标题下列出的文件将在首次下载后进行缓存
NETWORK - 在此标题下列出的文件需要与服务器的连接，且不会被缓存
FALLBACK - 在此标题下列出的文件规定当页面无法访问时的回退页面（比如 404 页面）

CACHE MANIFEST
第一行，CACHE MANIFEST，是必需的：
CACHE MANIFEST
/theme.css
/logo.gif
/main.js
上面的 manifest 文件列出了三个资源：一个 CSS 文件，一个 GIF 图像，以及一个 JavaScript 文件。当 manifest 文件被加载后，浏览器会从网站的根目录下载这三个文件。然后，无论用户何时与因特网断开连接，这些资源依然可用。

NETWORK
下面的 NETWORK 部分规定文件 "login.php" 永远不会被缓存，且离线时是不可用的：
NETWORK:
login.asp
可以使用星号来指示所有其他其他资源/文件都需要因特网连接：
NETWORK:
*

FALLBACK
下面的 FALLBACK 部分规定如果无法建立因特网连接，则用 "offline.html" 替代 /html/ 目录中的所有文件：
FALLBACK:
/html/ /offline.html
注释：第一个 URI 是资源，第二个是替补。

更新缓存
一旦应用被缓存，它就会保持缓存直到发生下列情况：
用户清空浏览器缓存
manifest 文件被修改（参阅下面的提示）
由程序来更新应用缓存
```

### HTML Server-Sent 事件：
```
Server-Sent 事件指的是网页自动从服务器获得更新。以前也可能做到这一点，前提是网页不得不询问是否有可用的更新。通过 Server-Sent 事件，更新能够自动到达。例如：Facebook/Twitter 更新、股价更新、新的博文、赛事结果，等等。

接收 Server-Sent 事件通知
EventSource 对象用于接收服务器发送事件通知：
var source = new EventSource("demo_sse.php");
source.onmessage = function(event) {
    document.getElementById("result").innerHTML += event.data + "<br>";
};
例子解释：
创建一个新的 EventSource 对象，然后规定发送更新的页面的 URL（本例中是 "demo_sse.php"）；
每当接收到一次更新，就会发生 onmessage 事件；
当 onmessage 事件发生时，把已接收的数据推入 id 为 "result" 的元素中。

服务器端代码实例
为了使上例运行，您需要能够发送数据更新的服务器（比如 PHP 或 ASP）。服务器端事件流的语法非常简单。请把 "Content-Type" 报头设置为 "text/event-stream"。现在，您可以开始发送事件流了。
PHP 中的代码 (demo_sse.php)：
<?php
header('Content-Type: text/event-stream');
header('Cache-Control: no-cache');
$time = date('r');
echo "data: The server time is: {$time}\n\n";
flush();
?>
ASP 中的代码 (VB) (demo_sse.asp)：
<%
Response.ContentType = "text/event-stream"
Response.Expires = -1
Response.Write("data: The server time is: " & now())
Response.Flush()
%>
代码解释：
把报头 "Content-Type" 设置为 "text/event-stream"；
规定不对页面进行缓存；
输出要发送的日期（始终以 "data: " 开头）；
向网页刷新输出数据。

EventSource 对象
在上例中，我们使用 onmessage 事件来获取消息。不过还可以使用其他事件：
事件	          描述
onopen	          当通往服务器的连接被打开
onmessage	  当接收到消息
onerror	          当发生错误
```