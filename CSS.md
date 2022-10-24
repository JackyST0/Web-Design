# CSS：

### 语法：
```
CSS 规则集（rule-set）由选择器和声明块组成,选择器指向您需要设置样式的 HTML 元素,声明块包含一条或多条用分号分隔的声明,每条声明都包含一个 CSS 属性名称和一个值，以冒号分隔,多条 CSS 声明用分号分隔,声明块用花括号括起来。
```

### 选择器：
```
CSS 元素选择器，元素选择器根据元素名称来选择 HTML 元素。
CSS id 选择器，id 选择器使用 HTML 元素的 id 属性来选择特定元素，元素的 id 在页面中是唯一的，因此 id 选择器用于选择一个唯一的元素！要选择具有特定 id 的元素，请写一个井号（＃），后跟该元素的 id。（注：id 名称不能以数字开头。）
CSS 类选择器，类选择器选择有特定 class 属性的 HTML 元素，如需选择拥有特定 class 的元素，请写一个句点（.）字符，后面跟类名。（注：类名不能以数字开头！）
CSS 通用选择器，通用选择器（*）选择页面上的所有的 HTML 元素。
CSS 分组选择器，分组选择器选取所有具有相同样式定义的 HTML 元素，如需对选择器进行分组，请用逗号来分隔每个选择器。
```

### 样式表：
```
外部 CSS，通过使用外部样式表，您只需修改一个文件即可改变整个网站的外观，每张 HTML 页面必须在 head 部分的` <link>` 元素内
包含对外部样式表文件的引用，外部样式表可以在任何文本编辑器中编写，并且必须以 .css 扩展名保存，外部 .css 文件不应包含任
何 HTML 标签。（注：请勿在属性值和单位之间添加空格（例如 margin-left: 20 px;）。正确的写法是：margin-left: 20px;）
内部 CSS，如果一张 HTML 页面拥有唯一的样式，那么可以使用内部样式表，内部样式是在 head 部分的` <style> `元素中进行定义。
行内 CSS，行内样式（也称内联样式）可用于为单个元素应用唯一的样式，如需使用行内样式，请将 style 属性添加到相关元素。style 
属性可包含任何 CSS 属性。
多个样式表，如果在不同样式表中为同一选择器（元素）定义了一些属性，则将使用最后读取的样式表中的值。
层叠顺序优先级：1.行内样式（在 HTML 元素中）；2.外部和内部样式表（在 head 部分）；3.浏览器默认样式。
```

### 注释：
```
注释用于解释代码，以后在您编辑源代码时可能会有所帮助，浏览器会忽略注释，格式是以 /* 开始，以 */结束。
```

### 颜色：
```
RGB 值，在 CSS 中，可以使用下面的公式将颜色指定为 RGB 值：rgb(red, green, blue)，每个参数 (red、green 以及 blue) 定义了0 到 255 之间的颜色强度。
RGBA 值,RGBA 颜色值是具有 alpha 通道的 RGB 颜色值的扩展 - 它指定了颜色的不透明度，RGBA 颜色值指定为：rgba(red, green, blue, alpha)，alpha 参数是介于 0.0（完全透明）和 1.0（完全不透明）之间的数字。
HEX 值，在 CSS 中，可以使用以下格式的十六进制值指定颜色：#rrggbb，其中 rr（红色）、gg（绿色）和 bb（蓝色）是介于 00 和 ff 之间的十六进制值（与十进制 0-255 相同）。
HSL 值,在 CSS 中，可以使用色相、饱和度和明度来指定颜色，格式如下：hsl(hue, saturation, lightness)
色相（hue）是色轮上从 0 到 360 的度数，0 是红色，120 是绿色，240 是蓝色；
饱和度（saturation）是一个百分比值，0％ 表示灰色阴影，而 100％ 是全色；
亮度（lightness）也是百分比，0％ 是黑色，50％ 是既不明也不暗，100％是白色。
HSLA 值，HSLA 颜色值是带有 Alpha 通道的 HSL 颜色值的扩展 - 它指定了颜色的不透明度，HSLA 颜色值指定为：hsla(hue, saturation,lightness, alpha)，alpha 参数是介于 0.0（完全透明）和 1.0（完全不透明）之间的数字。
```

### 背景：
```
不透明度 / 透明度，opacity 属性指定元素的不透明度/透明度，取值范围为 0.0 - 1.0，值越低，越透明。（注：使用 opacity 属性为元素
的背景添加透明度时，其所有子元素都继承相同的透明度。这可能会使完全透明的元素内的文本难以阅读。）

 属性	                      描述
background-attachment	    设置背景图像是固定的还是与页面的其余部分一起滚动。
background-clip	            规定背景的绘制区域。
background-color	    设置元素的背景色。
background-image	    设置元素的背景图像。
background-origin	    规定在何处放置背景图像。
background-position	    设置背景图像的开始位置。
background-repeat	    设置背景图像是否及如何重复。
background-size	            规定背景图像的尺寸。
background	            在一条声明中设置所有背景属性的简写属性。

在使用简写属性时，属性值的顺序为：
background-color
background-image
background-repeat
background-attachment
background-position
属性值之一缺失并不要紧，只要按照此顺序设置其他值即可。
```

### 边框：
```
border-style 属性指定要显示的边框类型。
允许以下值：
dotted - 定义点线边框
dashed - 定义虚线边框
solid - 定义实线边框
double - 定义双边框
groove - 定义 3D 坡口边框。效果取决于 border-color 值
ridge - 定义 3D 脊线边框。效果取决于 border-color 值
inset - 定义 3D inset 边框。效果取决于 border-color 值
outset - 定义 3D outset 边框。效果取决于 border-color 值
none - 定义无边框
hidden - 定义隐藏边框

border-style 属性可以设置一到四个值（用于上边框、右边框、下边框和左边框）。
它的工作原理是这样的（border-width和border-color 也同样适用）：
如果 border-style 属性设置四个值：
border-style: dotted solid double dashed;
上边框是虚线
右边框是实线
下边框是双线
左边框是虚线

如果 border-style 属性设置三个值：
border-style: dotted solid double;
上边框是虚线
右和左边框是实线
下边框是双线

如果 border-style 属性设置两个值：
border-style: dotted solid;
上和下边框是虚线
右和左边框是实线

如果 border-style 属性设置一个值：
border-style: dotted;
四条边均为虚线

单独的边，在 CSS 中，还有一些属性可用于指定每个边框（顶部、右侧、底部和左侧）：
border-top-style；border-right-style；border-bottom-style；border-left-style

border-width 属性指定四个边框的宽度，可以将宽度设置为特定大小（以 px、pt、cm、em 计），也可以使用以下三个预定义值之一：thin、medium 或 thick。
border-width 属性可以设置一到四个值（用于上边框、右边框、下边框和左边框）。

border-color 属性用于设置四个边框的颜色。（注：如果未设置 border-color，则它将继承元素的颜色。）
可以通过以下方式设置颜色：
name - 指定颜色名，比如 "red"
HEX - 指定十六进制值，比如 "#ff0000"
RGB - 指定 RGB 值，比如 "rgb(255,0,0)"
HSL - 指定 HSL 值，比如 "hsl(0, 100%, 50%)"
border-color 属性可以设置一到四个值（用于上边框、右边框、下边框和左边框）。

border 属性是以下各个边框属性的简写属性：
border-width
border-style（必需）
border-color

border-radius 属性用于向元素添加圆角边框。
```

### 外边距：
```
单独的边，CSS 拥有用于为元素的每一侧指定外边距的属性：
margin-top；margin-right；margin-bottom；margin-left
所有外边距属性都可以设置以下值：
auto - 使元素在其容器中水平居中，然后，该元素将占据指定的宽度，并且剩余空间将在左右边界之间平均分配
length - 以 px、pt、cm 等单位指定外边距
% - 指定以包含元素宽度的百分比计的外边距
inherit - 指定应从父元素继承外边距
提示：允许负值。

margin 属性是以下各外边距属性的简写属性：
margin-top
margin-right
margin-bottom
margin-left

如果 margin 属性有四个值：
margin: 25px 50px 75px 100px;
上外边距是 25px
右外边距是 50px
下外边距是 75px
左外边距是 100px

如果 margin 属性设置三个值：
margin: 25px 50px 75px;
上外边距是 25px
右和左外边距是 50px
下外边距是 75px

如果 margin 属性设置两个值：
margin: 25px 50px;
上和下外边距是 25px
右和左外边距是 50px

如果 margin 属性设置了一个值：
margin: 25px;
所有四个外边距都是 25px

外边距合并，简单地说，外边距合并指的是，当两个垂直外边距相遇时，它们将形成一个外边距，合并后的外边距的高度等于两个发生合并的外边距的高度中的较大者：
当一个元素出现在另一个元素上面时，第一个元素的下外边距与第二个元素的上外边距会发生合并；
当一个元素包含在另一个元素中时（假设没有内边距或边框把外边距分隔开），它们的上和/或下外边距也会发生合并；
假设有一个空元素，它有外边距，但是没有边框或填充。在这种情况下，上外边距与下外边距就碰到了一起，它们会发生合并。（如果这个外边距遇到另一个元素的外边距，它还会发生合并）
```

### 内边距：
```
单独的边，CSS 拥有用于为元素的每一侧指定内边距的属性：
padding-top
padding-right
padding-bottom
padding-left
所有内边距属性都可以设置以下值：
length - 以 px、pt、cm 等单位指定内边距
% - 指定以包含元素宽度的百分比计的内边距
inherit - 指定应从父元素继承内边距
提示：不允许负值。

padding 属性是以下各内边距属性的简写属性：
padding-top
padding-right
padding-bottom
padding-left

工作原理是这样的：
如果 padding 属性有四个值：
padding: 25px 50px 75px 100px;
上内边距是 25px
右内边距是 50px
下内边距是 75px
左内边距是 100px

如果 padding 属性设置了三个值：
padding: 25px 50px 75px;
上内边距是 25px
右和左内边距是 50px
下内边距是 75px

如果 padding 属性设置了两个值：
padding: 25px 50px;
上和下内边距是 25px
右和左内边距是 50px

如果 padding 属性设置了一个值：
padding: 25px;
所有四个内边距都是 25px

CSS width 属性指定元素内容区域的宽度，内容区域是元素（盒模型）的内边距、边框和外边距内的部分，因此，如果元素拥有指定的宽度，则添加到该元素的内边距会添加到元素的总宽度中，这通常是不希望的结果。
（若要保持宽度不变，无论填充量如何，那么您可以使用 box-sizing 属性，这将导致元素保持其宽度。如果增加内边距，则可用的内容空间会减少。）
```

### 高度和宽度：
```
height 和 width 属性用于设置元素的高度和宽度。（注：height 和 width 属性不包括内边距、边框或外边距。它设置的是元素内边距、边框以及外边距内的区域的高度或宽度。）
height 和 width 属性可设置如下值：
auto - 默认。浏览器计算高度和宽度。
length - 以 px、cm 等定义高度/宽度。
% - 以包含块的百分比定义高度/宽度。
initial - 将高度/宽度设置为默认值。
inherit - 从其父值继承高度/宽度。

max-width 属性用于设置元素的最大宽度，可以用长度值（例如 px、cm 等）或包含块的百分比（％）来指定 max-width（最大宽度），也可以将其设置为 none（默认值。意味着没有最大宽度）。
（注：max-width 属性的值将覆盖 width（宽度）。）
```

### 轮廓：
```
轮廓是在元素周围绘制的一条线，在边框之外，以凸显元素。(注：轮廓与边框不同！不同之处在于轮廓是在元素边框之外绘制的，并且可能与其他内容重叠，同样，轮廓也不是元素尺寸的一部分；元素的总宽度和高度不受轮廓线宽度的影响。)
CSS 拥有如下轮廓属性：
outline-style
outline-color
outline-width
outline-offset
outline

outline-style 属性指定轮廓的样式，并可设置如下值：
dotted - 定义点状的轮廓。
dashed - 定义虚线的轮廓。
solid - 定义实线的轮廓。
double - 定义双线的轮廓。
groove - 定义 3D 凹槽轮廓。
ridge - 定义 3D 凸槽轮廓。
inset - 定义 3D 凹边轮廓。
outset - 定义 3D 凸边轮廓。
none - 定义无轮廓。
hidden - 定义隐藏的轮廓。

outline-width 属性指定轮廓的宽度，并可设置如下值之一：
thin（通常为 1px）
medium（通常为 3px）
thick （通常为 5px）
特定尺寸（以 px、pt、cm、em 计）

outline-color 属性用于设置轮廓的颜色。
可以通过以下方式设置颜色：
name - 指定颜色名，比如 "red"
HEX - 指定十六进制值，比如 "#ff0000"
RGB - 指定 RGB 值，比如 "rgb(255,0,0)"
HSL - 指定 HSL 值，比如 "hsl(0, 100%, 50%)"
invert - 执行颜色反转（确保轮廓可见，无论是什么颜色背景）

outline 属性是用于设置以下各个轮廓属性的简写属性：
outline-width
outline-style（必需）
outline-color
outline 属性可指定一个、两个或三个值，值的顺序无关紧要。

outline-offset 属性在元素的轮廓与边框之间添加空间，元素及其轮廓之间的空间是透明的。
```

### 文本：
```
color 属性用于设置文本的颜色。颜色由以下值指定：
颜色名 - 比如 "red"
十六进制值 - 比如 "#ff0000"
RGB 值 - 比如 "rgb(255,0,0)"

text-align 属性用于设置文本的水平对齐方式，文本可以左对齐（left）或右对齐(right)，或居中对齐(center)，当 text-align 属性设置为 "justify" 后，将拉伸每一行，以使每一行具有相等的宽度，并且左右边距是直的.
direction 和 unicode-bidi 属性可用于更改元素的文本方向。
vertical-align 属性设置元素的垂直对齐方式。

text-decoration 属性用于设置或删除文本装饰；text-decoration: none，通常用于从链接上删除下划线；其他 text-decoration 值用于装饰文本如下：
text-decoration: overline - 上划线
text-decoration: line-through - 删除线
text-decoration: underline - 下划线

text-transform 属性用于指定文本中的大写和小写字母，它可用于将所有内容转换为大写或小写字母，或将每个单词的首字母大写：
text-transform: uppercase - 整体大写
text-transform: lowercase - 整体小写
text-transform: capitalize - 首字母大写

text-indent 属性用于指定文本第一行的缩进。
letter-spacing 属性用于指定文本中字符之间的间距。
line-height 属性用于指定行之间的间距。
word-spacing 属性用于指定文本中单词之间的间距。
white-space 属性指定元素内部空白的处理方式。

text-shadow 属性为文本添加阴影：
最简单的用法是只指定水平阴影（2px）和垂直阴影（2px）：text-shadow: 2px 2px;
接下来，向阴影添加颜色（红色）：text-shadow: 2px 2px red;
然后，向阴影添加模糊效果（5px）：text-shadow: 2px 2px 5px red；
```

### 字体：
```
在 CSS 中，有五个通用字体族：
衬线字体（Serif）- 在每个字母的边缘都有一个小的笔触。它们营造出一种形式感和优雅感。
无衬线字体（Sans-serif）- 字体线条简洁（没有小笔画）。它们营造出现代而简约的外观。
等宽字体（Monospace）- 这里所有字母都有相同的固定宽度。它们创造出机械式的外观。
草书字体（Cursive）- 模仿了人类的笔迹。
幻想字体（Fantasy）- 是装饰性/俏皮的字体。

通用字体族	                   字体名称实例
Serif                      Times New Roman；Georgia；Garamond
Sans-serif                 Arial；Verdana；Helvetica
Monospace	           Courier New；Lucida Console；Monaco
Cursive	                   Brush Script MT；Lucida Handwriting
Fantasy	                   Copperplate；Papyrus

font-family 属性应包含多个字体名称作为“后备”系统，以确保浏览器/操作系统之间的最大兼容性，请以您需要的字体开始，并以通用系列结束（如果没有其他可用字体，则让浏览器选择通用系列中的相似字体），字体名称应以逗号分隔。
（注：如果字体名称不止一个单词，则必须用引号引起来，例如："Times New Roman"。）

font-style 属性主要用于指定斜体文本。
此属性可设置三个值：
normal - 文字正常显示
italic - 文本以斜体显示
oblique - 文本为“倾斜”（倾斜与斜体非常相似，但支持较少）

font-weight 属性指定字体的粗细。
font-variant 属性指定是否以 small-caps 字体（小型大写字母）显示文本，在 small-caps 字体中，所有小写字母都将转换为大写字母。但是，转换后的大写字母的字体大小小于文本中原始大写字母的字体大小。

font-size 属性设置文本的大小。
用像素设置字体大小，使用像素设置文本大小可以完全控制文本大小；
用 em 设置字体大小，为了允许用户调整文本大小（在浏览器菜单中），许多开发人员使用 em 而不是像素。默认大小 1em 为 16px，可以使用这个公式从像素到 em 来计算大小：pixels/16=em；
用百分比和 Em 的组合设置字体大小，如：font-size: 2.5em;font-size: 1.875em;font-size: 0.875em;
用响应式字体大小，可以使用 vw 单位设置文本大小，它的意思是“视口宽度”（"viewport width"），这样，文本大小将遵循浏览器窗口的大小，请调整浏览器窗口的大小，以查看字体大小如何缩放。

font 属性是以下属性的简写属性（注：font-size 和 font-family 的值是必需，如果缺少其他值之一，则会使用其默认值。）：
font-style
font-variant
font-weight
font-size/line-height
font-family
```

### 链接：
```
链接可以使用任何 CSS 属性（例如 color、font-family、background 等）来设置样式，此外，可以根据链接处于什么状态来设置链接的不同样式。
四种链接状态分别是：
a:link - 正常的，未访问的链接
a:visited - 用户访问过的链接
a:hover - 用户将鼠标悬停在链接上时
a:active - 链接被点击时

如果为多个链接状态设置样式，请遵循如下顺序规则：
a:hover 必须 a:link 和 a:visited 之后
a:active 必须在 a:hover 之后
```

### 列表：
```
在 HTML 中，列表主要有两种类型：
无序列表（<ul>）- 列表项用的是项目符号标记
有序列表（<ol>）- 列表项用的是数字或字母标记
CSS 列表属性使您可以：
为有序列表设置不同的列表项标记
为无序列表设置不同的列表项标记
将图像设置为列表项标记
为列表和列表项添加背景色

list-style-type 属性指定列表项标记的类型。（注：有些值用于无序列表，而有些值用于有序列表。）
list-style-type:none 属性也可以用于删除标记/项目符号。
（注：列表还拥有默认的外边距和内边距，要删除此内容，请在 <ul> 或 <ol> 中添加 margin:0 和 padding:0 ）

list-style-image 属性将图像指定为列表项标记。

list-style-position 属性指定列表项标记（项目符号）的位置：
"list-style-position: outside;" 表示项目符号点将在列表项之外，列表项每行的开头将垂直对齐。（这是默认的）
"list-style-position: inside;" 表示项目符号将在列表项内，由于它是列表项的一部分，因此它将成为文本的一部分，并在开头推开文本。

在使用简写属性时，属性值的顺序为：
list-style-type（如果指定了 list-style-image，那么在由于某种原因而无法显示图像时，会显示这个属性的值）
list-style-position（指定列表项标记应显示在内容流的内部还是外部）
list-style-image（将图像指定为列表项标记）
如果缺少上述属性值之一，则将插入缺失属性的默认值（如果有）。
```

### 表格：
```
全宽表格，在某些情况下，表格似乎很小。如果您需要一个可以覆盖整个屏幕（全宽）的表格，请为 <table> 元素添加 width: 100%
合并表格边框，border-collapse 属性设置是否将表格边框折叠为单一边框：border-collapse: collapse;
可悬停表格，在 <tr> 元素上使用 :hover 选择器，以突出显示鼠标悬停时的表格行：tr:hover {background-color: #f5f5f5;}
条状表格，在 <tr> 元素上使用 :nth-child() 选择器，并为所有偶数（或奇数）表行添加 background-color：tr:nth-child(even) {background-color: #f2f2f2;}
响应式表格，在 <table> 元素周围添加带有 overflow-x:auto 的容器元素（例如 <div>），以实现响应式效果。
```

### display属性：
```
display 属性规定是否/如何显示元素，每个 HTML 元素都有一个默认的 display 值，具体取决于它的元素类型，大多数元素的默认 display 值为 block 或 inline。
块级元素总是从新行开始，并占据可用的全部宽度（尽可能向左和向右伸展）。
块级元素的一些例子：
html
<div>
<h1> - <h6>
<p>
<form>
<header>
<footer>
<section>
内联元素不从新行开始，仅占用所需的宽度。
行内元素的一些例子：
<span>
<a>
<img>

display: inline-block与 display: inline 相比，主要区别在于 display: inline-block 允许在元素上设置宽度和高度。
同样，如果设置了 display: inline-block，将保留上下外边距/内边距，而 display: inline 则不会。
display: inline-block与 display: block 相比，主要区别在于 display：inline-block 在元素之后不添加换行符，因此该元素可以位于其他元素旁边。
display 的一种常见用法：inline-block 用于水平而不是垂直地显示列表项。

display: none; 通常与 JavaScript 一起使用，以隐藏和显示元素，而无需删除和重新创建它们。
通过将 display 属性设置为 none 可以隐藏元素，该元素将被隐藏，并且不会占用任何空间；visibility:hidden; 也可以隐藏元素，但是，该元素仍将占用与之前相同的空间，元素将被隐藏，但仍会影响布局。
```

### position 属性：
```
position 属性规定应用于元素的定位方法的类型。
有五个不同的位置值：
static
relative
fixed
absolute
sticky
元素其实是使用 top、bottom、left 和 right 属性定位的。但是，除非首先设置了 position 属性，否则这些属性将不起作用。根据不同的 position 值，它们的工作方式也不同。

position: static - HTML 元素默认情况下的定位方式为 static（静态），静态定位的元素不受 top、bottom、left 和 right 属性的影响，position: static; 的元素不会以任何特殊方式定位；它始终根据页面的正常流进行定位。
position: relative - position: relative; 的元素相对于其正常位置进行定位，设置相对定位的元素的 top、right、bottom 和 left 属性将导致其偏离其正常位置进行调整。不会对其余内容进行调整来适应元素留下的任何空间。
position: fixed - position: fixed; 的元素是相对于视口定位的，这意味着即使滚动页面，它也始终位于同一位置， top、right、bottom 和 left 属性用于定位此元素，固定定位的元素不会在页面中通常应放置的位置上留出空隙。
position: absolute - position: absolute; 的元素相对于最近的定位祖先元素进行定位（而不是相对于视口定位，如 fixed），然而，如果绝对定位的元素没有祖先，它将使用文档主体（body），并随页面滚动一起移动。
position: sticky - position: sticky; 的元素根据用户的滚动位置进行定位，粘性元素根据滚动位置在相对（relative）和固定（fixed）之间切换。起先它会被相对定位，直到在视口中遇到给定的偏移位置为止 - 然后将其“粘贴”在适当的位置（比如 position:fixed）。

重叠元素，在对元素进行定位时，它们可以与其他元素重叠，z-index 属性指定元素的堆栈顺序（哪个元素应放置在其他元素的前面或后面），元素可以设置正或负的堆叠顺序。
```

### 溢出：
```
overflow 属性指定在元素的内容太大而无法放入指定区域时是剪裁内容还是添加滚动条。
overflow 属性可设置以下值：
visible - 默认。溢出没有被剪裁。内容在元素框外渲染
hidden - 溢出被剪裁，其余内容将不可见
scroll - 溢出被剪裁，同时添加滚动条以查看其余内容
auto - 与 scroll 类似，但仅在必要时添加滚动条
（注：overflow 属性仅适用于具有指定高度的块元素。）

overflow: visible - 默认情况下，溢出是可见的(visible)，这意味着它不会被裁剪，而是在元素框外渲染。
overflow: hidden - 如果使用 hidden 值，溢出会被裁剪，其余内容被隐藏。
overflow: scroll - 如果将值设置为 scroll，溢出将被裁剪，并添加滚动条以便在框内滚动，请注意，这将在水平和垂直方向上添加一个滚动条（即使您不需要它）。
overflow: auto - auto 值类似于 scroll，但是它仅在必要时添加滚动条。

overflow-x 和 overflow-y - overflow-x 和 overflow-y 属性规定是仅水平还是垂直地（或同时）更改内容的溢出：
overflow-x 指定如何处理内容的左/右边缘。
overflow-y 指定如何处理内容的上/下边缘。
```

### 浮动和清除：
```
float 属性用于定位和格式化内容，例如让图像向左浮动到容器中的文本那里。
float 属性可以设置以下值之一：
left - 元素浮动到其容器的左侧
right - 元素浮动在其容器的右侧
none - 默认值。元素不会浮动（将显示在文本中刚出现的位置）。
inherit - 元素继承其父级的 float 值
最简单的用法是，float 属性可实现（报纸上）文字包围图片的效果。

clear 属性指定哪些元素可以浮动于被清除元素的旁边以及哪一侧。
clear 属性可设置以下值之一：
none - 默认值。允许两侧都有浮动元素。
left - 左侧不允许浮动元素
right- 右侧不允许浮动元素
both - 左侧或右侧均不允许浮动元素
inherit - 元素继承其父级的 clear 值
使用 clear 属性的最常见用法是在元素上使用了 float 属性之后。
在清除浮动时，应该对清除与浮动进行匹配：如果某个元素浮动到左侧，则应清除左侧。您的浮动元素会继续浮动，但是被清除的元素将显示在其下方。
（注：如果一个元素比包含它的元素高，并且它是浮动的，它将“溢出”到其容器之外，然后我们可以向包含元素添加 overflow: auto;来解决此问题）
```

### 组合选择器：
```
选择器	                示例	        示例描述
element element	        div p	       选择 <div> 元素内的所有 <p> 元素。
element>element	        div > p	       选择其父元素是 <div> 元素的所有 <p> 元素。
element+element	        div + p	       选择所有紧随 <div> 元素之后的 <p> 元素。
element1~element2	p ~ ul	       选择前面有 <p> 元素的每个 <ul> 元素。
```

### 伪类：
```   
选择器	                             例子	                          例子描述
:active	                             a:active	                         选择活动链接变换的样式。
:checked	                     input:checked	                 选择每个被选中的 <input> 元素。
:disabled	                     input:disabled	                 选择每个被禁用的 <input> 元素。
:empty	                             p:empty	                         选择没有子元素的每个 <p> 元素。
:enabled	                     input:enabled	                 选择每个已启用的 <input> 元素。
:first-child	                     p:first-child	                 选择作为其父的首个子元素的每个 <p> 元素。
:first-of-type	                     p:first-of-type	                 选择作为其父的首个 <p> 元素的每个 <p> 元素。
:focus	                             input:focus	                 选择获得焦点的 <input> 元素。
:hover	                             a:hover	                         选择鼠标悬停其上的链接。
:in-range	                     input:in-range	                 选择具有指定范围内的值的 <input> 元素。
:invalid	                     input:invalid	                 选择所有具有无效值的 <input> 元素。
:lang(language)	                     p:lang(it)	                         选择每个 lang 属性值以 "it" 开头的 <p> 元素。
:last-child	                     p:last-child	                 选择作为其父的最后一个子元素的每个 <p> 元素。
:last-of-type	                     p:last-of-type	                 选择作为其父的最后一个 <p> 元素的每个 <p> 元素。
:link	                             a:link	                         选择所有未被访问的链接。
:not(selector)	                     :not(p)	                         选择每个非 <p> 元素的元素。
:nth-child(n)	                     p:nth-child(2)	                 选择作为其父的第二个子元素的每个 <p> 元素。
:nth-last-child(n)	             p:nth-last-child(2)	         选择作为父的第二个子元素的每个<p>元素，从最后一个子元素计数。
:nth-last-of-type(n)	             p:nth-last-of-type(2)	         选择作为父的第二个<p>元素的每个<p>元素，从最后一个子元素计数
:nth-of-type(n)	                     p:nth-of-type(2)	                 选择作为其父的第二个 <p> 元素的每个 <p> 元素。
:only-of-type	                     p:only-of-type	                 选择作为其父的唯一 <p> 元素的每个 <p> 元素。
:only-child	                     p:only-child	                 选择作为其父的唯一子元素的 <p> 元素。
:optional	                     input:optional	                 选择不带 "required" 属性的 <input> 元素。
:out-of-range	                     input:out-of-range	                 选择值在指定范围之外的 <input> 元素。
:read-only	                     input:read-only	                 选择指定了 "readonly" 属性的 <input> 元素。
:read-write	                     input:read-write	                 选择不带 "readonly" 属性的 <input> 元素。
:required	                     input:required	                 选择指定了 "required" 属性的 <input> 元素。
:root	                             root	                         选择元素的根元素。
:target	                             #news:target	                 选择当前活动的 #news 元素（单击包含该锚名称的 URL）。
:valid	                             input:valid	                 选择所有具有有效值的 <input> 元素。
:visited	                     a:visited	                         选择所有已访问的链接。
```

### 伪元素：
```
选择器	            例子	            例子描述
::after	            p::after	           在每个 <p> 元素之后插入内容。（配合content：一起使用）
::before	    p::before	           在每个 <p> 元素之前插入内容。（配合content：一起使用）
::first-letter 	    p::first-letter	   选择每个 <p> 元素的首字母。
::first-line	    p::first-line	   选择每个 <p> 元素的首行。
::selection	    p::selection	   选择用户选择的元素部分。
```

### 属性选择器：
```
选择器	                   例子	                            例子描述
[attribute]	           [target]	                    选择带有 target 属性的所有元素。
[attribute=value]	   [target=_blank]	            选择带有 target="_blank" 属性的所有元素。
[attribute~=value]	   [title~=flower]	            选择带有包含 "flower" 一词的 title 属性的所有元素。
[attribute|=value]	   [lang|=en]	                    选择带有以 "en" 开头的 lang 属性的所有元素。
[attribute^=value]	   a[href^="https"]	            选择其 href 属性值以 "https" 开头的每个 <a> 元素。
[attribute$=value]	   a[href$=".pdf"]	            选择其 href 属性值以 ".pdf" 结尾的每个 <a> 元素。
[attribute*=value]	   a[href*="w3school"]	            选择其 href 属性值包含子串 "w3school" 的每个 <a> 元素。
```

### 计数器：
```
CSS 计数器就像“变量”。变量值可以通过 CSS 规则递增（将跟踪它们的使用次数）。
如需使用 CSS 计数器，我们将使用以下属性：
counter-reset - 创建或重置计数器
counter-increment - 递增计数器值
content - 插入生成的内容
counter() 或 counters() 函数 - 将计数器的值添加到元素
```

### 单位：
```
绝对长度：
绝对长度单位是固定的，用任何一个绝对长度表示的长度都将恰好显示为这个尺寸。
不建议在屏幕上使用绝对长度单位，因为屏幕尺寸变化很大。但是，如果已知输出介质，则可以使用它们，例如用于打印布局（print layout）。
单位	    描述	
cm	   厘米	 
mm	   毫米	
in	   英寸 (1in = 96px = 2.54cm)	
px*	   像素 (1px = 1/96th of 1in)	
pt	   点 (1pt = 1/72 of 1in)	
pc	   派卡 (1pc = 12 pt)	

相对长度
相对长度单位规定相对于另一个长度属性的长度。相对长度单位在不同渲染介质之间缩放表现得更好。
单位	    描述	
em	   相对于元素的字体大小（font-size）（2em 表示当前字体大小的 2 倍）	
ex	   相对于当前字体的 x-height(极少使用)	
ch	   相对于 "0"（零）的宽度	
rem	   相对于根元素的字体大小（font-size）	
vw	   相对于视口*宽度的 1%	
vh	   相对于视口*高度的 1%	
vmin       相对于视口*较小尺寸的 1％	
vmax       相对于视口*较大尺寸的 1％	
%	   相对于父元素	
```

### 特异性：
```
特异性层次
每个选择器在特异性层次结构中都有其位置。以下四种类别定义了选择器的特异性级别：
行内样式 - 行内（内联）样式直接附加到要设置样式的元素。实例：<h1 style="color: #ffffff;">。
ID - ID 是页面元素的唯一标识符，例如 #navbar。
类、属性和伪类 - 此类别包括 .classes、[attributes] 和伪类，例如：:hover、:focus 等。
元素和伪元素 - 此类别包括元素名称和伪元素，比如 h1、div、:before 和 :after。

如何计算特异性？
从 0 开始，为 style 属性添加 1000，为每个 ID 添加 100，为每个属性、类或伪类添加 10，为每个元素名称或伪元素添加 1。

请思考以下三个代码片段：
A: h1
B: #content h1
C: <div id="content"><h1 style="color: #ffffff">Heading</h1></div>
A 的特异性为 1（一个元素）
B 的特异性为 101（一个 ID 引用以及一个元素）
C 的特异性为 1000（行内样式）
由于 1 < 101 < 1000，因此第三条规则（C）具有更高的特异性，所以将被应用。

特异性规则 1：
在特异性相同的情况下：最新的规则很重要 - 如果将同一规则两次写入外部样式表，那么样式表中后面的规将更靠近要设置样式的元素，因此会被应用；
特异性规则 2：
ID 选择器比属性选择器拥有更高的特异性；
特异性规则 3：
上下文选择器比单一元素选择器更具体；
特异性规则 4：
类选择器会击败任意数量的元素选择器。
```

### 圆角：
```
CSS border-radius 属性定义元素角的半径。
border-radius 属性实际上是以下属性的简写属性：
border-top-left-radius - 定义左上角边框的形状。
border-top-right-radius	- 定义右上角边框的形状。
border-bottom-right-radius - 定义右下角边框的形状。
border-bottom-left-radius - 定义左下角边框的形状。

border-radius 属性可以接受一到四个值。规则如下：
四个值 - border-radius: 15px 50px 30px 5px;（依次分别用于：左上角、右上角、右下角、左下角）：
三个值 - border-radius: 15px 50px 30px;（第一个值用于左上角，第二个值用于右上角和左下角，第三个用于右下角）：
两个值 - border-radius: 15px 50px;（第一个值用于左上角和右下角，第二个值用于右上角和左下角）：
一个值 - border-radius: 15px;（该值用于所有四个角，圆角都是一样的）
```

### 边框属性：
```
CSS border-image 属性允许您指定要使用的图像，而不是包围普通边框。
该属性有三部分：
用作边框的图像；
在哪里裁切图像；
定义中间部分应重复还是拉伸。
（注：为了使 border-image 起作用，该元素还需要设置 border 属性！）

border-image 属性实际上是以下属性的简写属性：
border-image-source - 规定用作边框的图像的路径。
border-image-slice - 规定如何裁切边框图像。
border-image-width - 规定边框图像的宽度。
border-image-outset - 规定边框图像区域超出边框盒的量。
border-image-repeat - 规定边框图像应重复、圆角、还是拉伸。
```

### 多重背景：
```
CSS 允许您通过 background-image 属性为一个元素添加多幅背景图像，不同的背景图像用逗号隔开，并且图像会彼此堆叠，其中的第一幅图像最靠近观看者。

background-size 设置背景图片大小。图片可以保有其原有的尺寸，或者拉伸到新的尺寸，或者在保持其原有比例的同时缩放到元素的可用空间的尺寸。
background-size 属性可以接受多个值。规则如下：
/* 关键字 */
background-size: cover （cover 关键字会缩放背景图像，以使内容区域完全被背景图像覆盖（其宽度和高度均等于或超过内容区域）。这样，背景图像的某些部分可能在背景定位区域中不可见。）
background-size: contain （contain 关键字将背景图像缩放为尽可能大的尺寸（但其宽度和高度都必须适合内容区域）。这样，取决于背景图像和背景定位区域的比例，可能存在一些未被背景图像覆盖的背景区域。）
/* 一个值：这个值指定图片的宽度，图片的高度隐式的为 auto */
background-size: 50%
background-size: 3em
background-size: 12px
background-size: auto
/* 两个值：第一个值指定图片的宽度，第二个值指定图片的高度 */
background-size: 50% auto
background-size: 3em 25%
background-size: auto 6px
background-size: auto auto
/* 逗号分隔的多个值：设置多重背景 */
background-size: auto, auto     /* 不同于 background-size: auto auto */
background-size: 50%, 25%, 25%
background-size: 6px, auto, contain
/* 全局属性 */
background-size: inherit;
background-size: initial;
background-size: unset;

background-origin 属性指定背景图像的位置。
该属性接受三个不同的值：
border-box - 背景图片从边框的左上角开始
padding-box -背景图像从内边距边缘的左上角开始（默认）
content-box - 背景图片从内容的左上角开始

background-clip 属性指定背景的绘制区域。
该属性接受三个不同的值：
border-box - 背景绘制到边框的外部边缘（默认）
padding-box - 背景绘制到内边距的外边缘
content-box - 在内容框中绘制背景
```

### 渐变：
```
CSS 线性渐变，如需创建线性渐变，您必须定义至少两个色标。色标是您要呈现平滑过渡的颜色，您还可以设置起点和方向（或角度）以及渐变效果。
语法：background-image: linear-gradient(direction, color-stop1, color-stop2, ...);
线性渐变 - 从上到下（默认）
#grad {background-image: linear-gradient(red, yellow);}
线性渐变 - 从左到右
#grad {background-image: linear-gradient(to right, red , yellow);}
线性渐变 - 对角线
#grad {background-image: linear-gradient(to bottom right, red, yellow);}

使用角度，如果希望对渐变角度做更多的控制，您可以定义一个角度，来取代预定义的方向（向下、向上、向右、向左、向右下等等）。值 0deg 等于向上（to top）。值 90deg 等于向右（to right）。值 180deg 等于向下（to bottom）。
语法：background-image: linear-gradient(angle, color-stop1, color-stop2);

repeating-linear-gradient() 函数用于重复线性渐变。

CSS 径向渐变，径向渐变由其中心定义，如需创建径向渐变，您还必须定义至少两个色标。
语法：background-image: radial-gradient(shape size at position, start-color, ..., last-color);
默认地，shape 为椭圆形，size 为最远角，position 为中心。
设置形状，shape 参数定义形状。它可接受 circle 或 ellipse 值。默认值为 ellipse（椭圆）。

size 参数定义渐变的大小。它可接受四个值：
closest-side
farthest-side
closest-corner
farthest-corner
设置了不同 size 关键词的径向渐变：
#grad1 {background-image: radial-gradient(closest-side at 60% 55%, red, yellow, black);}
#grad2 {background-image: radial-gradient(farthest-side at 60% 55%, red, yellow, black);}

repeating-radial-gradient() 函数用于重复径向渐变。
```

### 阴影：
```
通过使用 CSS，您可以在文本和元素上添加阴影，如下属性：
text-shadow
box-shadow

text-shadow 属性为文本添加阴影，最简单的用法是只指定水平阴影（2px）和垂直阴影（2px）：h1 {text-shadow: 2px 2px;}
接下来，为阴影添加颜色：h1 {text-shadow: 2px 2px red;}
然后，向阴影添加模糊效果：h1 {text-shadow: 2px 2px 5px red;}

box-shadow 属性应用阴影于元素，最简单的用法是只指定水平阴影和垂直阴影：div {box-shadow: 10px 10px;}
接下来，为阴影添加颜色：div {box-shadow: 10px 10px grey;}
接下来，向阴影添加模糊效果：div {box-shadow: 10px 10px 5px grey;}
```

### 文本效果：
```
文字溢出,text-overflow 属性规定应如何向用户呈现未显示的溢出内容：
text-overflow: clip; - 被裁剪
text-overflow: ellipsis; - 将其呈现为省略号（...）
字换行,word-wrap 属性使长文字能够被折断并换到下一行：
word-wrap: break-word; - 强制对文本进行换行，即使这意味着在词中间将其拆分
换行规则,word-break 属性指定换行规则：
word-break: keep-all; - 将连字符打断
word-break: break-all; - 将在任何字符处中断
书写模式,writing-mode 属性规定文本行是水平放置还是垂直放置：
writing-mode: horizontal-tb - 水平书写
writing-mode: vertical-rl - 垂直书写
```

### web字体：
```
在 @font-face 规则中：首先定义字体的名称（例如 myFirstFont），然后指向该字体文件：
@font-face {
  font-family: myFirstFont;
  src: url(sansation_light.woff);
}
提示：字体 URL 始终使用小写字母。大写字母可能会在 IE 中产生意外结果。

下表列出了能够在 @font-face 规则内定义的所有字体描述符（font descriptor）：
描述符	                       值	                  描述
font-family	               name	                 必需。定义字体名称。
src	                       URL	                 必需。定义字体文件的 URL。
font-stretch	               normal                    可选。定义应如何拉伸字体。默认值是 "normal"。
                               condensed
                               ultra-condensed
                               extra-condensed
                               semi-condensed
                               expanded
                               semi-expanded
                               extra-expanded
                               ultra-expanded
font-style	               normal                     可选。定义字体的样式。默认值是 "normal"。
                               italic
                               oblique
font-weight	               normal                     可选。定义字体的粗细。默认值是 "normal"。
                               bold
                               100
                               200
                               300
                               400
                               500
                               600
                               700
                               800
                               900
unicode-range	               unicode-range	          可选。定义字体支持的 UNICODE 字符范围。默认值是 "U+0-10FFFF"。
```

### 2D转换：
```
通过使用 CSS transform 属性，您可以利用以下 2D 转换方法：
translate()
rotate()
scaleX()
scaleY()
scale()
skewX()
skewY()
skew()
matrix()

translate() 方法从其当前位置移动元素（根据为 X 轴和 Y 轴指定的参数），下面的例子把 <div> 元素从其当前位置向右移动 50 个像素，并向下移动 100 个像素：
div {transform: translate(50px, 100px);}
rotate() 方法根据给定的角度顺时针或逆时针旋转元素，下面的例子把 <div> 元素顺时针旋转 20 度：
div {transform: rotate(20deg);}
scale() 方法增加或减少元素的大小（根据给定的宽度和高度参数），下面的例子把 <div> 元素增大为其原始宽度的两倍和其原始高度的三倍：
div {transform: scale(2, 3);}
scaleX() 方法增加或减少元素的宽度，下面的例子把 <div> 元素增大为其原始宽度的两倍：
div {transform: scaleX(2);}
scaleY() 方法增加或减少元素的高度，下面的例子把 <div> 元素增大到其原始高度的三倍：
div {transform: scaleY(3);}
skewX() 方法使元素沿 X 轴倾斜给定角度，下例把 <div> 元素沿X轴倾斜 20 度：
div {transform: skewX(20deg);}
skewY() 方法使元素沿 Y 轴倾斜给定角度，下例把 <div> 元素沿 Y 轴倾斜 20 度：
div {transform: skewY(20deg);}
skew() 方法使元素沿 X 和 Y 轴倾斜给定角度，下面的例子使 <div> 元素沿 X 轴倾斜 20 度，同时沿 Y 轴倾斜 10 度：
div {transform: skew(20deg, 10deg);}
matrix() 方法把所有 2D 变换方法组合为一个，matrix() 方法可接受六个参数，其中包括数学函数，这些参数使您可以旋转、缩放、移动（平移）和倾斜元素。
参数如下：matrix(scaleX(),skewY(),skewX(),scaleY(),translateX(),translateY())
div {transform: matrix(1, -0.3, 0, 1, 0, 0);}
```

### 3D转换：
```
通过 CSS transform 属性，您可以使用以下 3D 转换方法：
rotateX()
rotateY()
rotateZ()

rotateX() 方法使元素绕其 X 轴旋转给定角度：
#myDiv {transform: rotateX(150deg);}
rotateY() 方法使元素绕其 Y 轴旋转给定角度：
#myDiv {transform: rotateY(130deg);}
rotateZ() 方法使元素绕其 Z 轴旋转给定角度：
#myDiv {transform: rotateZ(90deg);}
```

### 过渡：
```
如需创建过渡效果，必须明确两件事：
您要添加效果的 CSS 属性
效果的持续时间
（注：如果未规定持续时间部分，则过渡不会有效果，因为默认值为 0。）
下面的例子展示了 100px * 100px 的红色 <div> 元素。 <div> 元素还为 width 属性指定了过渡效果，持续时间为 2 秒：
div {
  width: 100px;
  height: 100px;
  background: red;
  transition: width 2s;
}

transition-timing-function 属性规定过渡效果的速度曲线，transition-timing-function 属性可接受以下值：
ease - 规定过渡效果，先缓慢地开始，然后加速，然后缓慢地结束（默认）
linear - 规定从开始到结束具有相同速度的过渡效果
ease-in -规定缓慢开始的过渡效果
ease-out - 规定缓慢结束的过渡效果
ease-in-out - 规定开始和结束较慢的过渡效果
cubic-bezier(n,n,n,n) - 允许您在三次贝塞尔函数中定义自己的值

transition-delay 属性规定过渡效果的延迟（以秒计），下例在启动之前有 1 秒的延迟：
div {transition-delay: 1s;}

属性	                     描述
transition	                简写属性，用于将四个过渡属性设置为单一属性。
transition-delay	        规定过渡效果的延迟（以秒计）。
transition-duration	        规定过渡效果要持续多少秒或毫秒。
transition-property	        规定过渡效果所针对的 CSS 属性的名称。
transition-timing-function	规定过渡效果的速度曲线。
```

### 动画：
```
如果您在 @keyframes 规则中指定了 CSS 样式，动画将在特定时间逐渐从当前样式更改为新样式，要使动画生效，必须将动画绑定到某个元素。
animation-name 属性规定 @keyframes 动画的名称。
animation-duration 属性定义需要多长时间才能完成动画。如果未指定 animation-duration 属性，则动画不会发生，因为默认值是 0s（0秒）。
下面的例子将 "example" 动画绑定到 <div> 元素。动画将持续 4 秒钟，同时将 <div> 元素的背景颜色从 "red" 逐渐改为 "yellow"：
/* 动画代码 */
@keyframes example {
  from {background-color: red;}
  to {background-color: yellow;}
}
/* 向此元素应用动画效果 */
div {
  width: 100px;
  height: 100px;
  background-color: red;
  animation-name: example;
  animation-duration: 4s;
}
在上面的例子中，通过使用关键字 "from" 和 "to"（代表 0％（开始）和 100％（完成）），我们设置了样式何时改变，您也可以使用百分比值。通过使用百分比，您可以根据需要添加任意多个样式更改。

animation-delay 属性规定动画开始的延迟时间，负值也是允许的。如果使用负值，则动画将开始播放，如同已播放 N 秒。
animation-iteration-count 属性指定动画应运行的次数。

animation-direction 属性指定是向前播放、向后播放还是交替播放动画。
animation-direction 属性可接受以下值：
normal - 动画正常播放（向前）。默认值
reverse - 动画以反方向播放（向后）
alternate - 动画先向前播放，然后向后
alternate-reverse - 动画先向后播放，然后向前

animation-timing-function 属性规定动画的速度曲线。
animation-timing-function 属性可接受以下值：
ease - 指定从慢速开始，然后加快，然后缓慢结束的动画（默认）
linear - 规定从开始到结束的速度相同的动画
ease-in - 规定慢速开始的动画
ease-out - 规定慢速结束的动画
ease-in-out - 指定开始和结束较慢的动画
cubic-bezier(n,n,n,n) - 运行您在三次贝塞尔函数中定义自己的值

在不播放动画时（在开始之前，结束之后，或两者都结束时），animation-fill-mode 属性规定目标元素的样式。
animation-fill-mode 属性可接受以下值：
none - 默认值。动画在执行之前或之后不会对元素应用任何样式。
forwards - 元素将保留由最后一个关键帧设置的样式值（依赖 animation-direction 和 animation-iteration-count）。
backwards - 元素将获取由第一个关键帧设置的样式值（取决于 animation-direction），并在动画延迟期间保留该值。
both - 动画会同时遵循向前和向后的规则，从而在两个方向上扩展动画属性。

下例使用六种动画属性：
div {
  animation-name: example;
  animation-duration: 5s;
  animation-timing-function: linear;
  animation-delay: 2s;
  animation-iteration-count: infinite;
  animation-direction: alternate;
}
使用简写的 animation 属性也可以实现与上例相同的动画效果：
div {
  animation: example 5s linear 2s infinite alternate;
}
```

### object-fit属性：
```
CSS object-fit 属性用于规定应如何调整 <img> 或 <video> 的大小来适应其容器。
object-fit 属性可接受如下值：
fill - 默认值。调整替换后的内容大小，以填充元素的内容框。如有必要，将拉伸或挤压物体以适应该对象。
contain - 缩放替换后的内容以保持其纵横比，同时将其放入元素的内容框。
cover - 调整替换内容的大小，以在填充元素的整个内容框时保持其长宽比。该对象将被裁剪以适应。
none - 不对替换的内容调整大小。
scale-down - 调整内容大小就像没有指定内容或包含内容一样（将导致较小的具体对象尺寸）
```

### 多列：
```
column-count 属性规定元素应被划分的列数，下面的例子将 <div> 元素中的文本分为 3 列：
div {column-count: 3;}
column-gap 属性规定列之间的间隔，下面的例子指定列之间的间距为 40 像素：
div {column-gap: 40px;}
column-rule-style 属性规定列之间的规则样式：
div {column-rule-style: solid;}
column-rule-width 属性规定列之间的规则宽度：
div {column-rule-width: 1px;}
column-rule-color 属性规定列之间的规则的颜色：
div {column-rule-color: lightblue;}
column-rule 属性是用于设置上面所有 column-rule-* 属性的简写属性，下例设置了列之间的规则的宽度、样式和颜色：
div {column-rule: 1px solid lightblue;}
column-span 属性规定元素应跨越多少列，下例规定了<h2> 元素应跨所有列：
h2 {column-span: all;}
column-width 属性为列指定建议的最佳宽度，下例规定了列的建议最佳宽度应为 100px：
div {column-width: 100px;}
```

### 用户界面：
```
resize 属性规定元素是否应（以及如何）被用户调整大小。
resize: horizontal; - 允许用户在水平方向上调整元素的大小。
resize: vertical; - 允许用户在垂直方向上调整元素的大小。
resize: both; - 允许用户在水平和垂直方向上调整元素的大小。
resize: none; - 元素不能被用户缩放。
outline-offset 属性在轮廓与元素的边缘边框之间添加空间。
```

### 变量：
```
var() 函数用于插入 CSS 变量的值。var() 函数的语法：var(name, value)
值	           描述
name	         必需。变量名（以两条破折号开头）。
value	         可选。回退值（在未找到变量时使用）。
（注：变量名称必须以两个破折号（--）开头，且区分大小写！）

var() 如何工作
首先：CSS 变量可以有全局或局部作用域。
全局变量可以在整个文档中进行访问/使用，而局部变量只能在声明它的选择器内部使用。
如需创建具有全局作用域的变量，请在 :root 选择器中声明它。 :root 选择器匹配文档的根元素。
如需创建具有局部作用域的变量，请在将要使用它的选择器中声明它。

下面的例子使用 var() 函数，首先，我们声明两个全局变量（--blue 和 --white）。然后，我们使用 var() 函数稍后在样式表中插入变量的值：
:root {
  --blue: #1e90ff;
  --white: #ffffff;
}
body { background-color: var(--blue); }
h2 { border-bottom: 2px solid var(--blue); }

局部变量：有时，我们希望变量仅在页面的特定部分中进行更改，假设我们想要按钮元素使用不同的蓝色，那么，我们可以在 button 选择器内重新声明 --blue 变量，当我们在这个选择器中使用 var(--blue) 时，它将使用此处声明的局部 --blue 变量值，我们看到局部的 --blue 变量会覆盖 button 元素的全局 --blue 变量：
/* 此处定义变量为全局变量 */
:root {
  --blue: #1e90ff;
  --white: #ffffff;
}
button {
  --blue: #0000ff;/* 此处重新定义变量为局部变量，在此选择器内调用的变量都是此局部变量 */
  background-color: var(--white);
  color: var(--blue);
  border: 1px solid var(--blue);
  padding: 5px;
}
提示：如果只在一个地方使用一个变量，我们也可以声明一个新的局部变量。
```

### Box Sizing：
```
CSS box-sizing 属性允许我们在元素的总宽度和高度中包括内边距（填充）和边框。
默认情况下，元素的宽度和高度是这样计算的：
width + padding + border = 元素的实际宽度
height + padding + border = 元素的实际高度
这意味着：当您设置元素的宽度/高度时，该元素通常看起来比您设置的更大（因为元素的边框和内边距已被添加到元素的指定宽度/高度中）。

如果在元素上设置了 box-sizing: border-box;，则宽度和高度会包括内边距和边框：
.div1 {
  width: 300px;
  height: 100px;
  border: 1px solid blue;
  box-sizing: border-box;
}
.div2 {
  width: 300px;
  height: 100px;
  padding: 50px;
  border: 1px solid red;
  box-sizing: border-box;
}
由于使用 box-sizing: border-box; 的效果如此之好，许多开发人员希望页面上的所有元素都能够以这种方式工作。
```

### Flexbox：
```
在 Flexbox 布局模块（问世）之前，可用的布局模式有以下四种：
块（Block - 用于网页中的部分（节）
行内（Inline） - 用于文本
表 - 用于二维表数据
定位 - 用于元素的明确位置
弹性框布局模块，可以更轻松地设计灵活的响应式布局结构，而无需使用浮动或定位。

通过将 display 属性设置为 flex，flex 容器将可伸缩：
.flex-container {display: flex;}
以下是 flex 容器属性：
flex-direction
flex-wrap
flex-flow
justify-content
align-items
align-content

flex-direction 属性定义容器要在哪个方向上堆叠 flex 项目。
column 值设置垂直堆叠 flex 项目（从上到下）：
.flex-container {
  display: flex;
  flex-direction: column;
}
column-reverse 值垂直堆叠 flex 项目（但从下到上）。
row 值水平堆叠 flex 项目（从左到右）。
row-reverse 值水平堆叠 flex 项目（但从右到左）。

flex-wrap 属性规定是否应该对 flex 项目换行。
wrap 值规定 flex 项目将在必要时进行换行：
.flex-container {
  display: flex;
  flex-wrap: wrap;
}
nowrap 值规定将不对 flex 项目换行（默认）。
wrap-reverse 值规定如有必要，弹性项目将以相反的顺序换行。

flex-flow 属性是用于同时设置 flex-direction 和 flex-wrap 属性的简写属性。
.flex-container {
  display: flex;
  flex-flow: row wrap;
}

justify-content 属性用于水平对齐 flex 项目。
center 值将 flex 项目在容器的中心对齐：
.flex-container {
  display: flex;
  justify-content: center;
}
flex-start 值将 flex 项目在容器的开头对齐（默认）。
flex-end 值将 flex 项目在容器的末端对齐。
space-around 值显示行之前、之间和之后带有空格的 flex 项目。
space-between 值显示行之间有空格的 flex 项目。

align-items 属性用于垂直对齐 flex 项目。
center 值将 flex 项目在容器中间对齐：
.flex-container {
  display: flex;
  height: 200px;
  align-items: center;
}
flex-start 值将 flex 项目在容器顶部对齐。
flex-end 值将弹性项目在容器底部对齐。
stretch 值拉伸 flex 项目以填充容器（默认）。
baseline 值使 flex 项目基线对齐。

align-content 属性用于对齐弹性线。
space-between 值显示的弹性线之间有相等的间距：
.flex-container {
  display: flex;
  height: 600px;
  flex-wrap: wrap;
  align-content: space-between;
}
space-around 值显示弹性线在其之前、之间和之后带有空格。
stretch 值拉伸弹性线以占据剩余空间（默认）。
center 值在容器中间显示弹性线。
flex-start 值在容器开头显示弹性线。
flex-end 值在容器的末尾显示弹性线。

子元素（项目），flex 容器的直接子元素会自动成为弹性（flex）项目。
用于弹性项目的属性有：
order
flex-grow
flex-shrink
flex-basis
flex
align-self

order 属性规定 flex 项目的顺序。
代码中的首个 flex 项目不必在布局中显示为第一项。
order 值必须是数字，默认值是 0。
order 属性可以改变 flex 项目的顺序：
  <div style="order: 3">1</div>
  <div style="order: 2">2</div>
  <div style="order: 4">3</div> 
  <div style="order: 1">4</div>

flex-grow 属性规定某个 flex 项目相对于其余 flex 项目将增长多少。
该值必须是数字，默认值是 0。
使第三个弹性项目的增长速度比其他弹性项目快八倍：
  <div style="flex-grow: 1">1</div>
  <div style="flex-grow: 1">2</div>
  <div style="flex-grow: 8">3</div> 

flex-shrink 属性规定某个 flex 项目相对于其余 flex 项目将收缩多少。
该值必须是数字，默认值是 0。
  <div>1</div>
  <div>2</div>
  <div style="flex-shrink: 0">3</div>

flex-basis 属性规定 flex 项目的初始长度。
将第三个弹性项目的初始长度设置为 200 像素：
  <div>1</div>
  <div>2</div>
  <div style="flex-basis: 200px">3</div>

flex 属性是 flex-grow、flex-shrink 和 flex-basis 属性的简写属性。
使第三个弹性项目不可增长（0），不可收缩（0），且初始长度为 200 像素：
  <div>1</div>
  <div>2</div>
  <div style="flex: 0 0 200px">3</div>

align-self 属性规定弹性容器内所选项目的对齐方式。
align-self 属性将覆盖容器的 align-items 属性所设置的默认对齐方式。
把第三个弹性项目对齐到容器的中间：
  <div>1</div>
  <div>2</div>
  <div style="align-self: center">3</div>
```

### 媒体查询：
```
CSS2 中引入了 @media 规则，它让为不同媒体类型定义不同样式规则成为可能。
媒体查询语法
媒体查询由一种媒体类型组成，并可包含一个或多个表达式，这些表达式可以解析为 true 或 false。
@media not|only mediatype and (expressions) {
  CSS-Code;
}
下面的例子在视口宽度为 480 像素或更宽时将背景颜色更改为浅绿色（如果视口小于 480 像素，则背景颜色会是粉色）：
@media screen and (min-width: 480px) {
  body {
    background-color: lightgreen;
  }
}

方向：人像 / 风景，媒体查询还可以用于根据浏览器的方向更改页面的布局。
您可以设置一组 CSS 属性，这些属性仅在浏览器窗口的宽度大于其高度时才适用，即所谓的横屏：
如果方向处于横向模式，则使用浅蓝背景色：
@media only screen and (orientation: landscape) {
  body {
    background-color: lightblue;
  }
}

使用附加值，在下面的例子中，我们使用逗号（类似 OR 运算符）将附加的媒体查询添加到已有媒体查询中：
/* 当宽度在 600 像素到 900 像素之间或大于 1100 像素时 - 更改 <div> 的外观 */
@media screen and (max-width: 900px) and (min-width: 600px), (min-width: 1100px) {
  div.example {
    font-size: 50px;
    padding: 50px;
    border: 8px solid black;
    background: yellow;
  }
}
```

### 响应式网页设计：
```
视口（viewport）是用户在网页上的可见区域。
视口随设备而异，在移动电话上会比在计算机屏幕上更小。
在平板电脑和手机之前，网页仅设计为用于计算机屏幕，并且网页拥有静态设计和固定大小是很常见的。

设置视口，HTML5 引入了一种方法，使 Web 设计者可以通过 <meta> 标签来控制视口。
您应该在所有网页中包含以下 <meta> 视口元素：
<meta name="viewport" content="width=device-width, initial-scale=1.0">
它为浏览器提供了关于如何控制页面尺寸和缩放比例的指令。
width=device-width 部分将页面的宽度设置为跟随设备的屏幕宽度（视设备而定）。
当浏览器首次加载页面时，initial-scale=1.0 部分设置初始缩放级别。
```

### 网络布局模块：
```
当 HTML 元素的 display 属性设置为 grid 或 inline-grid 时，它就会成为网格容器。（网格容器的所有直接子元素将自动成为网格项目。）
grid-column-gap 属性设置列之间的间隙：
grid-column-gap: 50px;
grid-row-gap 属性设置行之间的间隙：
grid-row-gap: 50px;
grid-gap 属性是 grid-row-gap 和 grid-column-gap 属性的简写属性：
grid-gap: 50px 100px;
grid-gap 属性还可用于将行间隙和列间隙设置为一个值：
grid-gap: 50px;

网格行（Grid Lines），列之间的线称为列线（column lines），行之间的线称为行线（row lines）。
当把网格项目放在网格容器中时，请引用行号，把网格项目放在列线 1，并在列线 3 结束它：
.item1 {
  grid-column-start: 1;
  grid-column-end: 3;
}

grid-template-columns 属性定义网格布局中的列数，并可定义每列的宽度。
该值是以空格分隔的列表，其中每个值定义相应列的长度。
如果您希望网格布局包含 4 列，请指定这 4 列的宽度；如果所有列都应当有相同的宽度，则设置为 "auto"。
生成包含四列的网格：
grid-template-columns: auto auto auto auto;
（注：如果在 4 列网格中有 4 个以上的项目，则网格会自动添加新行并将这些项目放入其中。）
grid-template-columns 属性还可以用于指定列的尺寸（宽度）：
grid-template-columns: 80px 200px auto 40px;

grid-template-rows 属性定义每列的高度，它的值是以空格分隔的列表，其中每个值定义相应行的高度：
grid-template-rows: 80px 200px;

justify-content 属性用于在容器内对齐整个网格：（注：网格的总宽度必须小于容器的宽度，这样 justify-content 属性才能生效。）
justify-content: space-evenly; - 值 "space-evenly" 会在列之间以及列周围留出相等的空间：
提示：其他值的详情请看Flexbox板块。

align-content 属性用于垂直对齐容器内的整个网格：（注：网格的总高度必须小于容器的高度，这样 align-content 属性才能生效。）
align-content: space-evenly; - 值 "space-evenly" 将使行之间以及行周围具有相等的空间：
提示：其他值的详情请看Flexbox板块。

grid-column 属性定义将项目放置在哪一列上，您可以定义项目的开始位置以及结束位置，如需放置某个项目，您可以引用行号（line numbers），或使用关键字 "span" 来定义该项目将跨越多少列。（注：grid-column 属性是 grid-column-start 和 grid-column-end 属性的简写属性。）
使 "item1" 从第 1 列开始并在第 5 列之前结束：
.item1 {
  grid-column: 1 / 5;
}
使 "item1" 从第 1 列开始，并跨越 3 列：
.item1 {
  grid-column: 1 / span 3;
}

grid-row 属性定义了将项目放置在哪一行，您可以定义项目的开始位置以及结束位置，如需放置项目，您可以引用行号，或使用关键字 "span" 定义该项目将跨越多少行。（注：grid-row 属性是 grid-row-start 和 grid-row-end 属性的简写属性。）
使 "item1" 在 row-line 1 开始，在 row-line 4 结束：
.item1 {
  grid-row: 1 / 4;
}
使 "item1" 从第 1 行开始并跨越 2 行：
.item1 {
  grid-row: 1 / span 2;
}

grid-area 属性可以用作 grid-row-start、grid-column-start、grid-row-end 和 grid-column-end 属性的简写属性。
使 "item8" 从 row-line 1 和 column-line 2 开始，在 row-line 5 和 column line 6 结束：
.item8 {
  grid-area: 1 / 2 / 5 / 6;
}
使 "item8" 从 row-line 2 和 column-line 开始，并跨越 2 行和 3 列：
.item8 {
  grid-area: 2 / 1 / span 2 / span 3;
}

grid-area 属性也可以用于为网格项目分配名称。
可以通过网格容器的 grid-template-areas 属性来引用命名的网格项目。
item1 的名称是 "myArea"，并跨越五列网格布局中的所有五列：
.item1 {
  grid-area: myArea;
}
.grid-container {
  grid-template-areas: 'myArea myArea myArea myArea myArea';
}
每行由撇号（' '）定义，每行中的列都在撇号内定义，并以空格分隔。（注：句号表示没有名称的网格项目。）
```

