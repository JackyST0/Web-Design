# JavaScript:

### 简介：
```
getElementById() 是多个 JavaScript HTML 方法之一。

JavaScript 能够改变 HTML 内容，本例使用该方法来“查找” id="demo" 的 HTML 元素，并把元素内容（innerHTML）更改为 "Hello JavaScript"：
document.getElementById("demo").innerHTML = "Hello JavaScript"
提示：JavaScript 同时接受双引号和单引号。

JavaScript 能够改变 HTML 属性，本例通过改变 <img> 标签的 src 属性（source）来改变一张 HTML 图像：
document.getElementById('myImage').src='/i/eg_bulbon.gif'

JavaScript 能够改变 HTML 样式 (CSS)，改变 HTML 元素的样式，是改变 HTML 属性的一种变种：
document.getElementById("demo").style.fontSize = "25px";

JavaScript 能够隐藏 HTML 元素，可通过改变 display 样式来隐藏 HTML 元素：
document.getElementById("demo").style.display="none";

JavaScript 能够显示 HTML 元素，可通过改变 display 样式来显示隐藏的 HTML 元素：
document.getElementById("demo").style.display="block";
```

### 使用：
```
<script> 标签，在 HTML 中，JavaScript 代码必须位于 <script> 与 </script> 标签之间，您能够在 HTML 文档中放置任意数量的脚本，脚本可被放置与 HTML 页面的 <body> 或 <head> 部分中，或兼而有之：
<script>document.getElementById("demo").innerHTML = "我的第一段 JavaScript";</script>

外部脚本，脚本可放置与外部文件中，外部脚本很实用，如果相同的脚本被用于许多不同的网页。
JavaScript 文件的文件扩展名是 .js，如需使用外部脚本，请在 <script> 标签的 src (source) 属性中设置脚本的名称。（注：外部脚本不能包含 <script> 标签。）

在外部文件中放置脚本有如下优势：
分离了 HTML 和代码；
使 HTML 和 JavaScript 更易于阅读和维护；
已缓存的 JavaScript 文件可加速页面加载。
```

### 输出：
```
JavaScript 能够以不同方式“显示”数据：
使用 window.alert() - 写入警告框
使用 document.write() - 写入 HTML 输出
使用 innerHTML - 写入 HTML 元素
使用 console.log() - 写入浏览器控制台

使用 innerHTML
如需访问 HTML 元素，JavaScript 可使用 document.getElementById(id) 方法。
id 属性定义 HTML 元素，innerHTML 属性定义 HTML 内容。
提示：更改 HTML 元素的 innerHTML 属性是在 HTML 中显示数据的常用方法。
使用 document.write()
出于测试目的，使用 document.write() 比较方便。（注：在 HTML 文档完全加载后使用 document.write() 将删除所有已有的 HTML ）
提示：document.write() 方法仅用于测试。
使用 window.alert()
您能够使用警告框来显示数据。
使用 console.log()
在浏览器中，您可使用 console.log() 方法来显示数据。
通过 F12 来激活浏览器控制台，并在菜单中选择“控制台”查看数据。
```

### 语句：
```
在 HTML 中，JavaScript 语句是由 web 浏览器“执行”的“指令”。
关键词	                描述
break	               终止 switch 或循环。
continue	       跳出循环并在顶端开始。
debugger	       停止执行 JavaScript，并调用调试函数（如果可用）。
do ... while	       执行语句块，并在条件为真时重复代码块。
for	               标记需被执行的语句块，只要条件为真。
function	       声明函数。
if ... else	       标记需被执行的语句块，根据某个条件。
return	               退出函数。
switch	               标记需被执行的语句块，根据不同的情况。
try ... catch	       对语句块实现错误处理。
var	               声明变量。
（注：JavaScript 关键词指的是保留的单词。保留词无法用作变量名。）
```

### 语法：
```
JavaScript 语法是一套规则，它定义了 JavaScript 的语言结构。
JavaScript 注释，并非所有 JavaScript 语句都被“执行”，双斜杠 // 或 /* 与 */ 之间的代码被视为注释，注释会被忽略，不会被执行。

JavaScript 与驼峰式大小写，历史上，程序员曾使用三种把多个单词连接为一个变量名的方法：
连字符：
first-name, last-name, master-card, inter-city.
（注：JavaScript 中不能使用连字符，它是为减法预留的。）
下划线：
first_name, last_name, master_card, inter_city.
驼峰式大小写（Camel Case）：
FirstName, LastName, MasterCard, InterCity.
提示：JavaScript 程序员倾向于使用以小写字母开头的驼峰大小写：firstName, lastName, masterCard, interCity.

JavaScript 标识符，所有 JavaScript 变量必须以唯一的名称的标识，这些唯一的名称称为标识符，标识符可以是短名称（比如 x 和 y），或者更具描述性的名称（age、sum、totalVolume），构造变量名称（唯一标识符）的通用规则是：
名称可包含字母、数字、下划线和美元符号
名称必须以字母开头
名称也可以 $ 和 _ 开头（但是在本教程中我们不会这么做）
名称对大小写敏感（y 和 Y 是不同的变量）
保留字（比如 JavaScript 的关键词）无法用作变量名称
提示：JavaScript 标识符对大小写敏感。
```

### Let：
```
ES2015 引入了两个重要的 JavaScript 新关键词：let 和 const，这两个关键字在 JavaScript 中提供了块作用域（Block Scope）变量（和常量），在 ES2015 之前，JavaScript 只有两种类型的作用域：全局作用域和函数作用域。
全局作用域，全局（在函数之外）声明的变量拥有全局作用域，全局变量可以在 JavaScript 程序中的任何位置访问。
函数作用域，局部（函数内）声明的变量拥有函数作用域，局部变量只能在它们被声明的函数内访问。
块作用域。通过 var 关键词声明的变量没有块作用域，在块 {} 内声明的变量可以从块之外进行访问，在 ES2015 之前，JavaScript 是没有块作用域的，可以使用 let 关键词和const 关键词声明拥有块作用域的变量，在块 {} 内声明的变量无法从块外访问：
let x = 10;
// 此处 x 为 10
{ 
  let x = 6;
  // 此处 x 为 6
}
// 此处 x 为 10
HTML 中的全局变量，使用 JavaScript 的情况下，全局作用域是 JavaScript 环境，在 HTML 中，全局作用域是 window 对象，通过 var 关键词定义的全局变量属于 window 对象，通过 let 关键词和const 关键词定义的全局变量不属于 window 对象。
JavaScript const 变量必须在声明时赋值，如果我们将一个原始值赋给常量，我们就不能改变原始值，但我们可以更改常量对象的属性：
// 您可以创建 const 对象：
const car = {type:"porsche", model:"911", color:"Black"};
// 您可以更改属性：
car.color = "White";
// 您可以添加属性：
car.owner = "Bill";
```

### 算数：
```
算数运算符	描述
+	       加法
-	       减法
*	       乘法
**	       幂（ES2016）
/	       除法
%	       系数
++	       递增
--	       递减
+ 运算符也可用于对字符串进行相加（concatenate，级联）：
txt1 = "Bill";
txt2 = "Gates";
txt3 = txt1 + " " + txt2; 
txt3 的结果将是：
Bill Gates
```

### 赋值：
```
赋值运算符	例子	 等同于
=	       x = y	x = y
+=	       x += y	x = x + y
-=	       x -= y	x = x - y
*=	       x *= y	x = x * y
/=	       x /= y	x = x / y
%=	       x %= y	x = x % y
<<=	       x <<= y	x = x << y
>>=	       x >>= y	x = x >> y
>>>=	       x >>>= y	x = x >>> y
&=	       x &= y	x = x & y
^=	       x ^= y	x = x ^ y
|=	       x |= y	x = x | y
**=	       x **= y	x = x ** y
+= 赋值运算符也可用于相加（级联）字符串：
txt1 = "Hello ";
txt1 += "Kitty!"; 
txt1 的结果将是：
Hello Kitty!
```

### 数据类型：
```
JavaScript 变量能够保存多种数据类型：数值、字符串值、数组、对象等等。
JavaScript 字符串值，字符串（或文本字符串）是一串字符（比如 "Bill Gates"），字符串被引号包围。您可使用单引号或双引号。
JavaScript 数值，JavaScript 只有一种数值类型，写数值时用不用小数点均可。
JavaScript 布尔值，布尔值只有两个值：true 或 false。
JavaScript 数组，JavaScript 数组用方括号书写，数组的项目由逗号分隔。
JavaScript 对象，JavaScript 对象用花括号来书写。

Undefined，在 JavaScript 中，没有值的变量，其值是 undefined，typeof 也返回 undefined，任何变量均可通过设置值为 undefined 进行清空。其类型也将是 undefined。
空值，空值与 undefined 不是一回事，空的字符串变量既有值也有类型。
Null，在 JavaScript 中，null 是 "nothing"。它被看做不存在的事物，不幸的是，在 JavaScript 中，null 的数据类型是对象，您可以把 null 在 JavaScript 中是对象理解为一个 bug，它本应是 null，您可以通过设置值为 null 清空对象。
Undefined 与 Null 的区别，Undefined 与 null 的值相等，但类型不相等。

typeof 运算符，您可使用 JavaScript 的 typeof 来确定 JavaScript 变量的类型，typeof 运算符返回变量或表达式的类型。
原始数据，原始数据值是一种没有额外属性和方法的单一简单数据值。
typeof 运算符可返回以下原始类型之一：
string
number
boolean
undefined
复杂数据
typeof 运算符可返回以下两种类型之一：
function
object
typeof 运算符把对象、数组或 null 返回 object。
typeof 运算符把函数返回function。
```

### 函数：
```
JavaScript 函数通过 function 关键词进行定义，其后是函数名和括号 ()，函数名可包含字母、数字、下划线和美元符号（规则与变量名相同），圆括号可包括由逗号分隔的参数，由函数执行的代码被放置在花括号中：
function name(参数 1, 参数 2, 参数 3) {
    要执行的代码
}
函数参数（Function parameters）是在函数定义中所列的名称，函数参数（Function arguments）是当调用函数时由函数接收的真实的值。
```

### 对象：
```
对象也是变量。但是对象包含很多值，这段代码把多个值（porsche, 911, white）赋给名为 car 的变量：
var car = {type:"porsche", model:"911", color:"white"};
值以名称:值对的方式来书写（名称和值由冒号分隔），JavaScript 对象是被命名值的容器。
对象中的名称被称为对象属性，值被称为对象属性值。

在函数定义中，this 引用该函数的“拥有者”，在下面的例子中，this 指的是“拥有” fullName 函数的 person 对象，换言之，this.firstName 的意思是 this 对象的 firstName 属性：
var person = {
  firstName: "Bill",
  lastName : "Gates",
  id       : 678,
  fullName : function() {
    return this.firstName + " " + this.lastName;
  }
};

访问对象属性，您能够以两种方式访问属性：objectName.propertyName或者objectName["propertyName"]；
访问对象方法，您能够通过如下语法访问对象方法：objectName.methodName()。（注：如果您不使用 () 访问方法，则将返回函数定义）

请不要把字符串、数值和布尔值声明为对象！
如果通过关键词 "new" 来声明 JavaScript 变量，则该变量会被创建为对象：
var x = new String();        // 把 x 声明为 String 对象
var y = new Number();        // 把 y 声明为 Number 对象
var z = new Boolean();       //	把 z 声明为 Boolean 对象
请避免字符串、数值或逻辑对象。他们会增加代码的复杂性并降低执行速度。
```

### 字符串：
```
反斜杠转义字符（\）把特殊字符转换为字符串字符：
代码	  结果	    描述
\'	   '	   单引号
\"	   "	   双引号
\\	   \	   反斜杠
转义字符（\）也可用于在字符串中插入其他特殊字符。
其他六个 JavaScript 中有效的转义序列：
代码	    结果
\b	   退格键
\f	   换页
\n	   新行
\r	   回车
\t	   水平制表符
\v	   垂直制表符

字符串可以是对象,通常，JavaScript 字符串是原始值，通过字面方式创建：var firstName = "Bill";但是字符串也可通过关键词 new 定义为对象：
var firstName = new String("Bill")，当使用 == 相等运算符时，相等字符串是相等的：
var x = "Bill";             
var y = new String("Bill");
// (x == y) 为 true，因为 x 和 y 的值相等
当使用 === 运算符时，相等字符串是不相等的，因为 === 运算符需要类型和值同时相等。
var x = "Bill";             
var y = new String("Bill");
// (x === y) 为 false，因为 x 和 y 的类型不同（字符串与对象）
```

### 字符串方法：
```
length 属性返回字符串的长度：
var txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
var sln = txt.length;     // 返回 26

indexOf() 方法通过从前往后查的方式返回字符串中指定文本首次出现的索引（位置），lastIndexOf() 方法则通过从后往前查的方式返回指定文本在字符串中最后一次出现的索引：
var str = "The full name of China is the People's Republic of China.";
var pos = str.indexOf("China");    // 返回 17
JavaScript 从零计算位置，0 是字符串中的第一个位置，1 是第二个，2 是第三个 ...，如果未找到文本， indexOf() 和 lastIndexOf() 均返回 -1，两种方法都接受作为检索起始位置的第二个参数：
var str = "The full name of China is the People's Republic of China.";
var pos = str.indexOf("China", 18);   // 返回 51
（注：lastIndexOf()方法虽然是从后往前搜索，但返回的位置是从前开始数数和计算的，所以结果和indexOf()方法返回的相同）
search() 方法搜索特定值的字符串，并返回匹配的位置：
var str = "The full name of China is the People's Republic of China.";
var pos = str.search("China");      // 返回 17
indexOf() 与 search()区别在于：
search() 方法无法设置第二个开始位置参数。
indexOf() 方法无法设置更强大的搜索值（正则表达式）。

slice() 提取字符串的某个部分并在新字符串中返回被提取的部分，该方法设置两个参数：起始索引（开始位置），终止索引（结束位置），这个例子裁剪字符串中位置 7 到位置 13 的片段：
var str = "Apple, Banana, Mango";
var res = str.slice(7,13);       // 返回 Banana
如果某个参数为负，则从字符串的结尾开始计数，这个例子裁剪字符串中位置 -12 到位置 -6 的片段：
var str = "Apple, Banana, Mango";
var res = str.slice(-13,-7);     // 返回 Banana
（注：从后开始计数是从1开始数起）
如果省略第二个参数，则该方法将裁剪字符串的剩余部分：var res = str.slice(7);
substring() 类似于 slice()，不同之处在于 substring() 无法接受负的索引：
var str = "Apple, Banana, Mango";
var res = str.substring(7,13);     // 返回 Banana
如果省略第二个参数，则该 substring() 将裁剪字符串的剩余部分。
substr() 类似于 slice()，不同之处在于第二个参数规定被提取部分的长度，且第二个参数不能为负，因为它定义的是长度：
var str = "Apple, Banana, Mango";
var res = str.substr(7,6);       // 返回 Banana
如果省略第二个参数，则该 substr() 将裁剪字符串的剩余部分，如果首个参数为负，则从字符串的结尾计算位置。

replace() 方法用另一个值替换在字符串中指定的值，replace() 方法不会改变调用它的字符串，它返回的是新字符串：
str = "Please visit Microsoft!";
var n = str.replace("Microsoft", "W3School");      // 返回Please visit W3School!
默认地，replace() 只替换首个匹配；默认地，replace() 对大小写敏感，因此不对匹配 MICROSOFT。
如需执行大小写不敏感的替换，请使用正则表达式 /i（大小写不敏感）：var n = str.replace(/MICROSOFT/i, "W3School");
如需替换所有匹配，请使用正则表达式的 g 标志（用于全局搜索）：var n = str.replace(/Microsoft/g, "W3School");
（注：正则表达式不带引号。）

通过 toUpperCase() 把字符串转换为大写，通过 toLowerCase() 把字符串转换为小写：
var text1 = "Hello World!";       // 字符串
var text2 = text1.toUpperCase();  // text2 是被转换为大写的 text1
concat() 连接两个或多个字符串：
var text1 = "Hello";
var text2 = "World";
text3 = text1.concat(" ",text2);      // 返回 Hello World!
String.trim()，trim() 方法删除字符串两端的空白符：
var str = "       Hello World!        ";
alert(str.trim());       // 返回 Hello World!

charAt() 方法返回字符串中指定下标（位置）的字符串：
var str = "HELLO WORLD";
str.charAt(0);            // 返回 H
charCodeAt() 方法返回字符串中指定索引的字符 unicode 编码：
var str = "HELLO WORLD";
str.charCodeAt(0);         // 返回 72

可以通过 split() 将字符串转换为数组：
var txt = "a,b,c,d,e";   // 字符串
txt.split(",");          // 用逗号分隔
txt.split(" ");          // 用空格分隔
txt.split("|");          // 用竖线分隔
如果省略分隔符，被返回的数组将包含 index [0] 中的整个字符串；如果分隔符是 ""，被返回的数组将是间隔单个字符的数组：
var txt = "Hello";       // 字符串
txt.split("");           // 分隔为字符
```

### 字符串搜索：
```
String.match()，match() 方法根据正则表达式在字符串中搜索匹配项，并将匹配项作为 Array 对象返回，在字符串中搜索 "ain"：
let text = "The rain in SPAIN stays mainly in the plain";
text.match(/ain/g)    // 返回数组 [ain,ain,ain]
如果正则表达式不包含 g 修饰符（执行全局搜索），match() 方法将只返回字符串中的第一个匹配项。
语法：string.match(regexp)
参数          描述
regexp	     必需。需要搜索的值，为正则表达式。
返回          数组，包含匹配项，每个匹配项对应一个项目，若未找到匹配项，则为 null。

String.includes()，如果字符串包含指定值，includes() 方法返回 true：
let text = "Hello world, welcome to the universe.";
text.includes("world")    // 返回 true
语法：string.includes(searchvalue, start)
参数                描述
searchvalue	  必需。需要搜索的字符串。
start	          可选。默认为 0. 开始搜索的位置。
返回：	          如果字符串包含该值则返回 true，否则返回 false。
JS 版本：	   ES6 (2015)

String.startsWith()，如果字符串以指定值开头，则 startsWith() 方法返回 true，否则返回 false，检查字符串是否以 "Hello" 开头：
let text = "Hello world, welcome to the universe.";
text.startsWith("Hello")   // 返回 true
语法：string.startsWith(searchvalue, start)
参数	          描述
searchvalue	  必需。需要搜索的值。
start	          可选。默认为 0。开始搜索的位置。
（注：startsWith() 方法区分大小写。）

String.endsWith()，如果字符串以指定值结尾，则 endsWith() 方法返回 true，否则返回 false，检查字符串是否以 "Gates" 结尾：
var text = "Bill Gates";
text.endsWith("Gates")    // 返回 true
语法：string.endsWith(searchvalue, length)
参数	          描述
searchvalue	 必需。需要搜索的值。
length	         可选。要搜索的长度。
（注：endsWith() 方法区分大小写。）
```

### 字符串模板：
```
模板字面量使用反引号 (``) 而不是引号 ("") 来定义字符串：
let text = `Hello World!`;
模板字面量允许字符串中的变量：
let firstName = "Bill";
let lastName = "Gates";
let text = `Welcome ${firstName}, ${lastName}!`;
模板字面量允许字符串中的表达式：
let price = 10;
let VAT = 0.25;
let total = `Total: ${(price * (1 + VAT)).toFixed(2)}`;
用真实值自动替换表达式称为字符串插值。
```

### 数字：
```
JavaScript 数值始终是 64 位的浮点数，与许多其他编程语言不同，JavaScript 不会定义不同类型的数，比如整数、短的、长的、浮点的等等，JavaScript 数值始终以双精度浮点数来存储，根据国际 IEEE 754 标准，此格式用 64 位存储数值，其中 0 到 51 存储数字（片段），52 到 62 存储指数，63 位存储符号：
值(aka Fraction/Mantissa)	         指数	                          符号
52 bits(0 - 51)	                   11 bits (52 - 62)	           1 bit (63)

精度
整数（不使用指数或科学计数法）会被精确到 15 位：
var x = 999999999999999;   // x 将是 999999999999999
var y = 9999999999999999;  // y 将是 10000000000000000
小数的最大数是 17 位，但是浮点的算数并不总是 100% 精准：
var x = 0.2 + 0.1;         // x 将是 0.30000000000000004

数字和字符串相加
如果您对两个数相加，结果将是一个数；如果对两个字符串相加，结果将是一个字符串的级联；如果您对一个数和一个字符串相加，结果也是字符串级联；如果您对一个字符串和一个数字相加，结果也是字符串级联，常见的错误：
var x = 10;
var y = 20;
var z = "结果是： " + x + y;    // 返回 结果是：1020
原因是因为字符串在先，所以结果会发生字符串级联。
var x = 10;
var y = 20;
var z = "30";
var result = x + y + z;      // 返回 3030
原因是x 和 y 都是数，10 + 20 将被相加，z 是字符串，30 + "30" 被级联。

NaN 属于 JavaScript 保留词，指示某个数不是合法数，尝试用一个非数字字符串进行除法会得到 NaN（Not a Number）：
var x = 100 / "Apple";  // x 将是 NaN（Not a Number）
NaN 是数，typeof NaN 返回 number。
您可使用全局 JavaScript 函数 isNaN() 来确定某个值是否是数：
var x = 100 / "Apple";
isNaN(x);               // 返回 true，因为 x 不是数

Infinity （或 -Infinity）是 JavaScript 在计算数时超出最大可能数范围时返回的值，除以 0（零）也会生成 Infinity：
var x =  2 / 0;          // x 将是 Infinity
var y = -2 / 0;          // y 将是 -Infinity
Infinity 是数：typeOf Infinity 返回 number。

JavaScript 会把前缀为 0x 的数值常量解释为十六进制：
var x = 0xFF;             // x 将是 255。
绝不要用前导零写数字（比如 07），一些 JavaScript 版本会把带有前导零的数解释为八进制。默认地，Javascript 把数显示为十进制小数，但是您能够使用 toString() 方法把数输出为十六进制、八进制或二进制：
var myNumber = 128;
myNumber.toString(16);     // 返回 80
myNumber.toString(8);      // 返回 200
myNumber.toString(2);      // 返回 10000000
```

### 数字方法：
```
toString() 以字符串返回值，所有数字方法可用于任意类型的数字（字面量、变量或表达式）：
var x = 123;
x.toString();            // 从变量 x 返回 123
(123).toString();        // 从文本 123 返回 123
(100 + 23).toString();   // 从表达式 100 + 23 返回 123

toExponential() 返回字符串值，它包含已被四舍五入并使用指数计数法的数字，参数定义小数点后的字符数：
var x = 9.656;
x.toExponential(2);     // 返回 9.66e+0
x.toExponential(4);     // 返回 9.6560e+0
x.toExponential(6);     // 返回 9.656000e+0
（）参数是可选的。如果您没有设置它，JavaScript 不会对数字进行舍入。

toFixed() 返回字符串值，它包含了指定位数小数的数字：
var x = 9.656;
x.toFixed(0);           // 返回 10
x.toFixed(2);           // 返回 9.66
x.toFixed(4);           // 返回 9.6560
x.toFixed(6);           // 返回 9.656000
toFixed(2) 非常适合处理金钱。

toPrecision() 返回字符串值，它包含了指定长度的数字：
var x = 9.656;
x.toPrecision();        // 返回 9.656
x.toPrecision(2);       // 返回 9.7
x.toPrecision(4);       // 返回 9.656
x.toPrecision(6);       // 返回 9.65600

valueOf() 以原始值返回值：
var x = 123;
x.valueOf();            // 从变量 x 返回 123
(123).valueOf();        // 从文本 123 返回 123
(100 + 23).valueOf();   // 从表达式 100 + 23 返回 123

把变量转换为数值
方法	          描述
Number()	  返回数字，由其参数转换而来。
parseFloat()	  解析一段字符串并返回浮点数。允许空格。只返回首个数字。
parseInt()	  解析一段字符串并返回整数。允许空格。只返回首个数字。
（注：如果无法转换为数值，则返回 NaN (Not a Number)）

数值属性
属性                              描述
MAX_VALUE	                返回 JavaScript 中可能的最大数。
MIN_VALUE	                返回 JavaScript 中可能的最小数。
NEGATIVE_INFINITY	        表示负的无穷大（溢出返回）。
NaN	                        表示非数字值（"Not-a-Number"）。
POSITIVE_INFINITY	        表示无穷大（溢出返回）。
（注：数字属性属于名为 number 的 JavaScript 数字对象包装器，这些属性只能作为 Number.MAX_VALUE 访问，使用 myNumber.MAX_VALUE，其中 myNumber 是变量、表达式或值，将返回 undefined）
```

### 数组：
```
创建数组
使用数组文本是创建 JavaScript 数组最简单的方法，语法：
var array-name = [item1, item2, ...];
使用 JavaScript 关键词 new，下面的例子也会创建数组，并为其赋值：
var cars = new Array("Saab", "Volvo", "BMW");
以上两个例子效果完全一样，无需使用 new Array()，出于简洁、可读性和执行速度的考虑，请使用第一种方法（数组文本方法）。

length 属性返回数组的长度（数组元素的数目）：
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.length;                       // fruits 的长度是 4
添加数组元素，向数组添加新元素的最佳方法是使用 push() 方法：
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.push("Lemon");                // 向 fruits 添加一个新元素 (Lemon)
也可以使用 length 属性向数组添加新元素：
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits[fruits.length] = "Lemon";     // 向 fruits 添加一个新元素 (Lemon)
（注：添加最高索引的元素可在数组中创建未定义的“洞”）
```

### 数组方法：
```
join() 方法可将所有数组元素结合为一个字符串。它的行为类似 toString()，但是您还可以规定分隔符：
var fruits = ["Banana", "Orange","Apple", "Mango"];
document.getElementById("demo").innerHTML = fruits.join(" * ");       // 返回 Banana * Orange * Apple * Mango

在处理数组时，删除元素和添加新元素是很简单的，Popping 和 Pushing 指的是：从数组弹出项目，或向数组推入项目。
pop() 方法从数组中删除最后一个元素：
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.pop();              // 从 fruits 删除最后一个元素（"Mango"），返回值为"被弹出"的值
push() 方法（在数组结尾处）向数组添加一个新的元素：
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.push("Kiwi");       //  向 fruits 添加一个新元素，返回值为新数组的长度

位移元素，位移与弹出等同，但处理首个元素而不是最后一个，shift() 方法会删除首个数组元素，并把所有其他元素“位移”到更低的索引：
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.shift();            // 从 fruits 删除第一个元素 "Banana"，返回值为被"位移出"的值
unshift() 方法（在开头）向数组添加新元素，并“反向位移”旧元素：
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.unshift("Lemon");    // 向 fruits 添加新元素 "Lemon"，返回值为新数组的长度

删除元素，既然 JavaScript 数组属于对象，其中的元素就可以使用 JavaScript delete 运算符来删除：
var fruits = ["Banana", "Orange", "Apple", "Mango"];
delete fruits[0];           // 把 fruits 中的首个元素改为 undefined
使用 delete 会在数组留下未定义的空洞。请使用 pop() 或 shift() 取而代之。

拼接数组，splice() 方法可用于向数组添加新项：
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.splice(2, 2, "Lemon", "Kiwi");       // 返回 Banana,Orange,Lemon,Kiwi
第一个参数（2）定义了应添加新元素的位置（拼接），第二个参数（2）定义应删除多少元素，其余参数（“Lemon”，“Kiwi”）定义要添加的新元素，splice() 方法返回一个包含已删除项的数组。
使用 splice() 来删除元素，通过聪明的参数设定，您能够使用 splice() 在数组中不留“空洞”的情况下移除元素：
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.splice(0, 1);        // 删除 fruits 中的第一个元素
第一个参数（0）定义新元素应该被添加（接入）的位置，第二个参数（1）定义应该删除多个元素，其余参数被省略。没有新元素将被添加。

concat() 方法通过合并（连接）现有数组来创建一个新数组，concat() 方法不会更改现有数组。它总是返回一个新数组，concat() 方法可以使用任意数量的数组参数，concat() 方法也可以将值作为参数：
var arr1 = ["Cecilie", "Lone"];
var myChildren = arr1.concat(["Emil", "Tobias", "Linus"]);      // 返回 Cecilie, Lone，Emil, Tobias, Linus

slice() 方法用数组的某个片段切出新数组，slice() 方法创建新数组。它不会从源数组中删除任何元素，slice() 可接受两个参数，比如 (1, 3)。
该方法会从开始参数选取元素，直到结束参数（不包括）为止，如果结束参数被省略，则 slice() 会切出数组的剩余部分：
var fruits = ["Banana", "Orange", "Lemon", "Apple", "Mango"];
var citrus = fruits.slice(1, 3);       // 返回值 Orange,Lemon
```

### 数组排序：
```
sort() 方法以字母顺序对数组进行排序，reverse() 方法反转数组中的元素，您可以使用它以降序对数组进行排序：
var fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.sort();            // 对 fruits 中的元素进行排序，返回 Apple,Banana,Mango,Orange
fruits.reverse();         // 对已排序的 fruits 反转元素顺序，返回 Orange,Mango,Banana,Apple

数字按照字符串来排序，则 "25" 大于 "100"，因为 "2" 大于 "1"，正因如此，sort() 方法在对数值排序时会产生不正确的结果，我们通过一个比值函数来修正此问题，比较函数的目的是定义另一种排序顺序，比较函数应该返回一个负，零或正值，这取决于参数：
function(a, b){return a-b}
当 sort() 函数比较两个值时，会将值发送到比较函数，并根据所返回的值（负、零或正值）对这些值进行排序。
var points = [40, 100, 1, 5, 25, 10];
points.sort(function(a, b){return a - b});     // 执行升序操作，反之（ b - a ）为降序操作
当比较 40 和 100 时，sort() 方法会调用比较函数 function(40,100)，该函数计算 40-100，然后返回 -60（负值），排序函数将把 40 排序为比 100 更低的值。
同理，也可通过比值函数来查找最高（或最低）的数组值：
var points = [40, 100, 1, 5, 25, 10];
points.sort(function(a, b){return b - a});
// 现在 points[0] 包含最高值
// 而 points[points.length-1] 包含最低值
当然，您也可以使用 Math.max.apply 来查找数组中的最高值，使用 Math.min.apply 来查找数组中的最低值：
function myArrayMax(arr) {
    return Math.max.apply(null, arr);     // 返回最高值，反之 Math.min.apply 为最低值
}

排序对象数组，JavaScript 数组经常会包含对象：
var cars = [
{type:"Volvo", year:2016},
{type:"Saab", year:2001},
{type:"BMW", year:2010}];
即使对象拥有不同数据类型的属性，sort() 方法仍可用于对数组进行排序，解决方法是通过比较函数来对比属性值：
cars.sort(function(a, b){return a.year - b.year});
比较字符串属性会稍复杂：
cars.sort(function(a, b){
	  var x = a.type.toLowerCase();
	  var y = b.type.toLowerCase();
	  if (x < y) {return -1;}
	  if (x > y) {return 1;}
	  return 0;
});
```

### 数组迭代：
```
Array.forEach()
forEach() 方法为每个数组元素调用一次函数（回调函数）：
var txt = "";
var numbers = [45, 4, 9, 16, 25];                          // 返回 45 4 9 16 25       
numbers.forEach(myFunction);
function myFunction(value, index, array) {
  txt = txt + value + " ";                             
}
（注：该函数接受 3 个参数：项目值；项目索引；数组本身。当回调函数仅使用 value 参数时，可以省略索引和数组参数）

Array.map()
map() 方法通过对每个数组元素执行函数来创建新数组，map() 方法不会对没有值的数组元素执行函数，map() 方法不会更改原始数组，这个例子将每个数组值乘以2：
var numbers1 = [45, 4, 9, 16, 25];
var numbers2 = numbers1.map(myFunction);                     // 返回 90,8,18,32,50 
function myFunction(value, index, array) {
  return value * 2;                                  
}
（注：该函数接受 3 个参数：项目值；项目索引；数组本身。当回调函数仅使用 value 参数时，可以省略索引和数组参数）

Array.filter()
filter() 方法创建一个包含通过测试的数组元素的新数组，这个例子用值大于 18 的元素创建一个新数组：
var numbers = [45, 4, 9, 16, 25];
var over18 = numbers.filter(myFunction);                 // 返回 45,25
function myFunction(value, index, array) {
  return value > 18;
}
（注：该函数接受 3 个参数：项目值；项目索引；数组本身。当回调函数仅使用 value 参数时，可以省略索引和数组参数）

Array.reduce()
reduce() 方法在每个数组元素上运行函数，以生成（减少它）单个值，reduce() 方法在数组中从左到右工作，reduce() 方法不会减少原始数组，这个例子确定数组中所有数字的总和：
var numbers1 = [45, 4, 9, 16, 25];
var sum = numbers1.reduce(myFunction);                // 返回 99
function myFunction(total, value, index, array) {
  return total + value;
}
（注：此函数接受 4 个参数：总数（初始值/先前返回的值）；项目值；项目索引；数组本身。上例并未使用 index 和 array 参数，因此可以省略）
reduce() 方法能够接受一个初始值：var sum = numbers1.reduce(myFunction, 100);

Array.reduceRight()
reduceRight() 方法在每个数组元素上运行函数，以生成（减少它）单个值，reduceRight() 方法在数组中从右到左工作，，reduceRight() 方法不会减少原始数组，这个例子确定数组中所有数字的总和：
var numbers1 = [45, 4, 9, 16, 25];
var sum = numbers1.reduceRight(myFunction);                // // 返回 99
function myFunction(total, value, index, array) {
  return total + value;
}
（注：此函数接受 4 个参数：总数（初始值/先前返回的值）；项目值；项目索引；数组本身。上例并未使用 index 和 array 参数，因此可以省略）

Array.every()
every() 方法检查所有数组值是否通过测试,这个例子检查所有数组值是否大于 18：
var numbers = [45, 4, 9, 16, 25];
var allOver18 = numbers.every(myFunction);            // 返回 false
function myFunction(value, index, array) {
  return value > 18;
}
（注：该函数接受 3 个参数：项目值；项目索引；数组本身。当回调函数仅使用 value 参数时，可以省略索引和数组参数）

Array.some()
some() 方法检查某些数组值是否通过了测试，这个例子检查某些数组值是否大于 18：
var numbers = [45, 4, 9, 16, 25];
var someOver18 = numbers.some(myFunction);            // true
function myFunction(value, index, array) {
  return value > 18;
}
（注：该函数接受 3 个参数：项目值；项目索引；数组本身。当回调函数仅使用 value 参数时，可以省略索引和数组参数）

Array.find()
find() 方法返回通过测试函数的第一个数组元素的值,这个例子查找（返回）大于 18 的第一个元素的值：
var numbers = [4, 9, 16, 25, 29];
var first = numbers.find(myFunction);              // 返回 25
function myFunction(value, index, array) {
  return value > 18;
}
（注：该函数接受 3 个参数：项目值；项目索引；数组本身。当回调函数仅使用 value 参数时，可以省略索引和数组参数）

Array.findIndex()
findIndex() 方法返回通过测试函数的第一个数组元素的索引，这个例子查找大于 18 的第一个元素的索引：
var numbers = [4, 9, 16, 25, 29];
var first = numbers.findIndex(myFunction);         // 返回 3
function myFunction(value, index, array) {
  return value > 18;
}
（注：该函数接受 3 个参数：项目值；项目索引；数组本身。当回调函数仅使用 value 参数时，可以省略索引和数组参数）
```

### 数组const：
```
2015 年，JavaScript 引入了一个重要的新关键字：const，使用 const 声明数组已成为一种常见做法，用 const 声明的数组不能重新赋值但能更改常量数组的元素：
const cars = ["Saab", "Volvo", "BMW"];
cars = ["Toyota", "Volvo", "Audi"];    // ERROR
cars[0] = "Toyota";    // 更改第一个元素
JavaScript const 变量在声明时必须赋值，意思是：用 const 声明的数组必须在声明时进行初始化，使用 const 而不初始化数组是一个语法错误，不同于var 声明的数组可以随时初始化，且用 const 声明的数组具有块作用域：
const cars = ["Saab", "Volvo", "BMW"];
// 此处 cars[0] 为 "Saab"
{
  const cars = ["Toyota", "Volvo", "BMW"];
  // 此处 cars[0] 为 "Toyota"
}
// 此处 cars[0] 为 "Saab"
```

### 日期：
```
Date 对象由新的 Date() 构造函数创建，有 4 种方法创建新的日期对象：
new Date()
new Date(year, month, day, hours, minutes, seconds, milliseconds)
new Date(milliseconds)
new Date(date string)

new Date() 用当前日期和时间创建新的日期对象：
var d = new Date();
提示：日期对象是静态的。计算机时间正在滴答作响，但日期对象不会。

new Date(year, month, ...) 用指定日期和时间创建新的日期对象。（注：JavaScript 从 0 到 11 计算月份。一月是 0，十二月是11。）
7个数字分别指定年、月、日、小时、分钟、秒和毫秒（按此顺序）：
var d = new Date(2019, 12, 25, 10, 33, 30, 0);        // 返回 Sat Jan 25 2020 10:33:30 GMT+0800 (中國標準時間)
6个数字指定年、月、日、小时、分钟、秒：
var d = new Date(2019, 12, 25, 10, 33, 30);           // 返回 Sat Jan 25 2020 10:33:30 GMT+0800 (中國標準時間)
5个数字指定年、月、日、小时和分钟：
var d = new Date(2018, 11, 24, 10, 33);               // 返回 Mon Dec 24 2018 10:33:00 GMT+0800 (中國標準時間)
4个数字指定年、月、日和小时：
var d = new Date(2018, 11, 24, 10);                   // 返回 Mon Dec 24 2018 10:00:00 GMT+0800 (中國標準時間)
3 个数字指定年、月和日：
var d = new Date(2018, 11, 24);                       // 返回 Mon Dec 24 2018 00:00:00 GMT+0800 (中國標準時間)
2个数字指定年份和月份：
var d = new Date(2018, 11);                           // 返回 Sat Dec 01 2018 00:00:00 GMT+0800 (中國標準時間)
您不能省略月份。如果只提供一个参数，则将其视为毫秒。
var d = new Date(2018);                               // 返回 Thu Jan 01 1970 08:00:02 GMT+0800 (中國標準時間)
如果第一个数值为一位或两位数，年份将被解释为 19xx 年：
var d = new Date(99, 12, 25);                         // 返回 Tue Jan 25 2000 00:00:00 GMT+0800 (中國標準時間)
var d = new Date(9, 12, 25);                          // 返回 Tue Jan 25 1910 00:00:00 GMT+0800 (中國標準時間)

new Date(dateString) 从日期字符串创建一个新的日期对象：
var d = new Date("December 25, 2019 12:46:00");       // 返回 Wed Dec 25 2019 12:46:00 GMT+0800 (中國標準時間)

JavaScript 将日期存储为自 1970 年 1 月 1 日 00:00:00 UTC（协调世界时）以来的毫秒数，零时间是 1970 年 1 月 1 日 00:00:00 UTC，现在的时间你可以理解为是：1970 年 1 月 1 日之后的 n 毫秒。
new Date(milliseconds) 创建一个零时加毫秒的新日期对象：
var d = new Date(0);                                  // 返回 Thu Jan 01 1970 08:00:00 GMT+0800 (中國標準時間)
1970年 1 月 1 日加上100 000 000 000毫秒，大约是 1973 年 3 月 3 日：
var d = new Date(100000000000);                       // 返回 Sat Mar 03 1973 17:46:40 GMT+0800 (中國標準時間)
一天（24 小时）是 86 400 000 毫秒。
var d = new Date(86400000);                           // 返回 Fri Jan 02 1970 08:00:00 GMT+0800 (中國標準時間)

显示日期，JavaScript（默认情况下）将以全文本字符串格式输出日期：
Wed Mar 25 2015 08:00:00 GMT+0800 (中国标准时间)
在 HTML 中显示日期对象时，会使用 toString() 方法自动转换为字符串。
toUTCString() 方法将日期转换为 UTC 字符串（一种日期显示标准）：
var d = new Date();
document.getElementById("demo").innerHTML = d.toUTCString();            // 返回 Mon, 15 Aug 2022 07:43:42 GMT
toDateString() 方法将日期转换为更易读的格式：
var d = new Date();
document.getElementById("demo").innerHTML = d.toDateString();           // 返回 Mon Aug 15 2022
```

### 日期格式：
```
有四种 JavaScript 日期输入格式：
类型	         实例
ISO 日期	    "2018-02-19" （国际标准）
短日期	      "02/19/2018" 或者 "2018/02/19"
长日期	      "Feb 19 2018" 或者 "19 Feb 2019"
完整日期	    "Monday February 25 2015"
ISO 格式遵守 JavaScript 中的严格标准，其他格式不太明确，可能是浏览器特定的。

JavaScript ISO 日期
ISO 8601 是表现日期和时间的国际标准，ISO 8601 语法 (YYYY-MM-DD) 也是首选的 JavaScript 日期格式（完整日期）：
var d = new Date("2019-05-02");                  // 返回 Thu May 02 2019 08:00:00 GMT+0800 (中國標準時間)
提示：计算的日期相对于您的时区，根据您的时区，上面的结果将在 5 月 1 日至 5 月 2 日之间变化。
写日期也可以不规定具体某日 (YYYY-MM)：
var d = new Date("2019-05");                     // 返回 Wed May 01 2019 08:00:00 GMT+0800 (中國標準時間)
提示：时区会对结果在 4 月 30 日至 5 月 1 日之间产生变化。
写日期也可以不规定具体的月和日 (YYYY)：
var d = new Date("2018");                        // 返回 Mon Jan 01 2018 08:00:00 GMT+0800 (中國標準時間)
提示：时区会对结果在 2017 年 12 月 31 日至 2018 年 1 月 1 日之间产生变化。
写日期也可以添加时、分和秒 (YYYY-MM-DDTHH:MM:SS)：
var d = new Date("2019-05-02T12:00:00Z");         // 返回 Thu May 02 2019 20:00:00 GMT+0800 (中國標準時間)  
日期和时间通过大写字母 T 来分隔，UTC 时间通过大写字母 Z 来定义，如果您希望修改相对于 UTC 的时间，请删除 Z 并用 +HH:MM 或 -HH:MM 代替：
var d = new Date("2015-03-25T12:00:00-06:00");   // 返回 Thu Mar 26 2015 02:00:00 GMT+0800 (中國標準時間)
提示：UTC（Universal Time Coordinated）等同于 GMT（格林威治时间），UTC，协调世界时，又称世界统一时间，世界标准时间，国际协调时间，在日期-时间字符串中省略 T 或 Z，在不同浏览器中会产生不同结果。

JavaScript 短日期
短日期通常使用 "MM/DD/YYYY" 这样的语法：
var d = new Date("05/26/2019");                  // 返回 Sun May 26 2019 00:00:00 GMT+0800 (中國標準時間)
（注：在某些浏览器中，不带前导零的月或其会产生错误）

长日期通常以 "MMM DD YYYY" 这样的语法来写：
var d = new Date("Mar 26 2019");                 // 返回 Tue Mar 26 2019 00:00:00 GMT+0800 (中國標準時間)
提示：月和天能够以任意顺序出现，月能够以全称 (January) 或缩写 (Jan) 来写，逗号会被忽略，且对大小写不敏感。

JavaScript 完整日期
JavaScript 接受“完整 JavaScript 格式”的日期字符串：
var d = new Date("Mon Feb 19 2018 06:55:23 GMT+0100 (W. Europe Standard Time)");      // 返回 Mon Feb 19 2018 13:55:23 GMT+0800 (中國標準時間)
提示：JavaScript 会忽略日期名称和时间括号中的错误。
```

### 日期获取方法：
```
日期方法允许您获取并设置日期值（年、月、日、时、分、秒、毫秒），获取方法用于获取日期的某个部分（来自日期对象的信息）。下面是最常用的方法：
方法	              描述
getDate()	         以数字（1-31）返回日期的日
getDay()	         以数字（0-6）返回日期的星期名（weekday）
getFullYear()	     以四位数字形式返回日期年份
getHours()	       以数字（0-23）返回日期的小时数
getMilliseconds()	 以数字（0-999）返回日期的毫秒数
getMinutes()	     以数字（0-59）返回日期的分钟数
getMonth()	       以数字（0-11）返回日期的月份
getSeconds()	     以数字（0-59）返回日期的秒数
getTime()	         返回自 1970 年 1 月 1 日以来的毫秒数
```

### 日期设置方法：
```
使用“设置日期”方法可以设置日期对象的日期值（年、月、日、小时、分钟、秒、毫秒）。
setFullYear() 方法设置日期对象的年份。这个例子设置为 2020 年：
var d = new Date();
d.setFullYear(2020);
setFullYear() 方法可以选择设置月和日：
var d = new Date();
d.setFullYear(2020, 11, 3);
setMonth() 方法设置日期对象的月份（0-11）
setDate() 方法设置日期对象的日（1-31）：
var d = new Date();
d.setDate(15);
setDate() 方法也可用于将天数添加到日期：
var d = new Date();
d.setDate(d.getDate() + 50);
setHours() 方法设置日期对象的小时（0-23）
setMinutes() 方法设置日期对象的分钟（0-59）
setSeconds() 方法设置日期对象的秒数（0-59）

设置方法用于设置日期的某个部分。下面是最常用的方法：
方法	               描述
setDate()	          以数值（1-31）设置日
setFullYear()	      设置年（可选月和日）
setHours()	        设置小时（0-23）
setMilliseconds()	  设置毫秒（0-999）
setMinutes()	      设置分（0-59）
setMonth()	        设置月（0-11）
setSeconds()	      设置秒（0-59）
setTime()	          设置时间（从 1970 年 1 月 1 日至今的毫秒数）
```

### 数学：
```
JavaScript Math 对象允许您对数字执行数学任务。
Math.round(x) 的返回值是 x 四舍五入为最接近的整数：
Math.round(6.8);    // 返回 7
Math.round(2.3);    // 返回 2
Math.pow(x, y) 的返回值是 x 的 y 次幂：
Math.pow(8, 2);      // 返回 64
Math.sqrt(x) 返回 x 的平方根：
Math.sqrt(64);      // 返回 8
Math.abs(x) 返回 x 的绝对（正）值：
Math.abs(-4.7);     // 返回 4.7
Math.ceil(x) 的返回值是 x 上舍入最接近的整数：
Math.ceil(6.4);     // 返回 7
Math.floor(x) 的返回值是 x 下舍入最接近的整数：
Math.floor(2.7);    // 返回 2
Math.sin(x) 返回角 x（以弧度计）的正弦（介于 -1 与 1 之间的值）。
如果您希望使用角度替代弧度，则需要将角度转换为弧度：Angle in radians = Angle in degrees x PI / 180.
Math.sin(90 * Math.PI / 180);     // 返回 1（90 度的正弦）
Math.cos(x) 返回角 x（以弧度计）的余弦（介于 -1 与 1 之间的值）。
如果您希望使用角度替代弧度，则需要将角度转换为弧度：Angle in radians = Angle in degrees x PI / 180.
Math.cos(0 * Math.PI / 180);     // 返回 1（0 度的余弦）
Math.min() 和 Math.max() 可用于查找参数列表中的最低或最高值：
Math.min(0, 450, 35, 10, -8, -300, -78);  // 返回 -300
Math.max(0, 450, 35, 10, -8, -300, -78);  // 返回 450
Math.random() 返回介于 0（包括） 与 1（不包括） 之间的随机数：
Math.random();     // 返回随机数

Math 属性（常量）
JavaScript 提供了可由 Math 对象访问的 8 个数学常量：
Math.E          // 返回欧拉指数（Euler's number）
Math.PI         // 返回圆周率（约等于 3.141592653589793）
Math.SQRT2      // 返回 2 的平方根
Math.SQRT1_2    // 返回 1/2 的平方根
Math.LN2        // 返回 2 的自然对数
Math.LN10       // 返回 10 的自然对数
Math.LOG2E      // 返回以 2 为底的 e 的对数（约等于 1.414）
Math.LOG10E     // 返回以 10 为底的 e 的对数（约等于 0.434）
```

### 逻辑：
```
JavaScript 布尔（逻辑）代表两个值之一：true 或 false。
Boolean() 函数，您可以使用 Boolean() 函数来确定表达式（或变量）是否为真：
Boolean(10 > 9)        // 返回 true

所有具有“真实”值的即为 True：
var b1 = Boolean(100);                       // 返回 ture
var b2 = Boolean(3.14);                      // 返回 ture
var b3 = Boolean(-15);                       // 返回 ture
var b4 = Boolean("Hello");                   // 返回 ture
var b5 = Boolean('false');                   // 返回 ture
var b6 = Boolean(1 + 7 + 3.14);              // 返回 ture
所有不具有“真实”值的即为 False
0（零）的布尔值为 false：var x =Boolean(0);       // 返回 false
-0 （负零）的布尔值为 false：var x =Boolean(-0);       // 返回 false
""（空值）的布尔值为 false：var x =Boolean("");       // 返回 false
undefined（未定义） 的布尔值是 false：var x =Boolean(x);       // 返回 false
null 的布尔值是 false：var x =Boolean(null);       // 返回 false
NaN 的布尔值是 false：var x =Boolean(10/"H");       // 返回 false
```

### 比较：
```
比较运算符	    描述
==	           等于
===	           等值等型
!=	           不相等
!==	           不等值或不等型
>	           大于
<	           小于
>=	           大于或等于
<=	           小于或等于
?	           三元运算符
逻辑运算符	   描述
&&	           逻辑与
||	           逻辑或
!	           逻辑非

条件（三元）运算符，JavaScript 也包含了可基于某些条件向变量赋值的条件运算符。语法：
variablename = (condition) ? value1:value2
如果变量 age 的值小于 18，变量 voteable 的值将是 "太年轻"，否则变量 voteable 的值将是 "足够成熟":
var voteable = (age < 18) ? "太年轻":"足够成熟";
```

### 条件：
```
条件语句用于基于不同条件执行不同的动作，在 JavaScript 中，我们可使用如下条件语句：
使用 if 来规定要执行的代码块，如果指定条件为 true
使用 else 来规定要执行的代码块，如果相同的条件为 false
使用 else if 来规定要测试的新条件，如果第一个条件为 false
使用 switch 来规定多个被执行的备选代码块

if 语句
请使用 if 语句来规定假如条件为 true 时被执行的 JavaScript 代码块，语法：
if (条件) {
    如果条件为 true 时执行的代码
} 

else 语句
请使用 else 语句来规定假如条件为 false 时的代码块，语法：
if (条件) {
    条件为 true 时执行的代码块
} else { 
    条件为 false 时执行的代码块
}

else if 语句
请使用 else if 来规定当首个条件为 false 时的新条件，语法
if (条件 1) {
    条件 1 为 true 时执行的代码块
} else if (条件 2) {
    条件 1 为 false 而条件 2 为 true 时执行的代码块
 } else {
    条件 1 和条件 2 同时为 false 时执行的代码块
}

switch 语句用于基于不同条件执行不同动作。
请使用 switch 语句来选择多个需被执行的代码块之一，语法
switch(表达式) {
     case n:
        代码块
        break;
     case n:
        代码块
        break;
     default:
        默认代码块
} 
代码解释：计算一次 switch 表达式；把表达式的值与每个 case 的值进行对比；如果存在匹配，则执行关联代码。
break 关键词，如果 JavaScript 遇到 break 关键词，它会跳出 switch 代码块，此举将停止代码块中更多代码的执行以及 case 测试，如果找到匹配，并完成任务，则随机中断执行（break）。无需更多测试，break 能够节省大量执行时间，因为它会“忽略” switch 代码块中的其他代码的执行，不必中断 switch 代码块中的最后一个 case。代码块在此处会自然结束。
default 关键词，default 关键词规定不存在 case 匹配时所运行的代码，且默认的 case 不必是 switch 代码块中最后一个 case：
switch (new Date().getDay()) {
    default: 
        text = "期待周末！";
         break;
    case 6:
        text = "今天是周六";
        break; 
    case 0:
        text = "今天是周日";
} 
（注：如果 default 不是 switch 代码块中最后一个 case，请记得用 break 结束默认 case。）
常见的代码块，有时您会需要不同的 case 来使用相同的代码，在本例中，case 4 和 5 分享相同的代码块，而 0 和 6 分享另一段代码块：
switch (new Date().getDay()) {
    case 4:
    case 5:
        text = "周末快到了：）";
        break; 
    case 0:
    case 6:
        text = "今天是周末~";
         break;
    default: 
        text = "期待周末！";
} 
```

### 循环：
```
不同类型的循环，JavaScript 支持不同类型的循环：
for - 多次遍历代码块
for/in - 遍历对象属性
while - 当指定条件为 true 时循环一段代码块
do/while - 当指定条件为 true 时循环一段代码块

For 循环
for 循环是在您希望创建循环时经常使用的工具，for 循环的语法如下：
for (语句 1; 语句 2; 语句 3) {
     要执行的代码块
}
语句 1 在循环（代码块）开始之前执行；语句 2 定义运行循环（代码块）的条件；语句 3 会在循环（代码块）每次被执行后执行。
语句 1，通常，您会使用语句 1 来初始化循环中所使用的的变量（i = 0），但情况并不总是这样，JavaScript 不会在意。语句 1 是可选的，您可以在语句 1 中初始化多个值（由逗号分隔）：
for (i = 0, len = cars.length, text = ""; i < len; i++) { 
    text += cars[i] + "<br>";
}
而且您还可以省略语句 1（比如在循环开始前设置好值）：
var i = 2;
var len = cars.length;
var text = "";
for (; i < len; i++) { 
    text += cars[i] + "<br>";
}
语句 2，通常语句 2 用于计算初始变量的条件，但情况并不总是这样，JavaScript 不会在意。语句 2 也是可选的，如果语句 2 返回 true，那么循环会重新开始，如果返回 false，则循环将结束，如果省略语句 2，那么必须在循环中提供一个 break。否则循环永远不会结束。
语句 3，通常语句 3 会递增初始变量的值，但情况并不总是这样，JavaScript 不会在意。语句 3 也是可选的，语句 3 可做任何事情，比如负递增（i--），正递增（i = i + 15），或者任何其他事情，语句 3 也可被省略（比如当您在循环内递增值时）：
var i = 0;
var len = cars.length;
for (; i < len; ) { 
    text += cars[i] + "<br>";
      i++;
}

For In 循环
JavaScript for in 语句循环遍历对象或数组的属性，语法：
for (key/variable in object/array) {
  // code block to be executed
}
例子解释,for in 循环遍历 person 对象;每次迭代返回一个键 (x);键用于访问键的值;键的值为 person[x]:
const person = {fname:"Bill", lname:"Gates", age:25};
let text = "";
for (let x in person) {
  text += person[x];               // 返回 Bill Gates 19
}
提示：如果索引顺序很重要，请不要在数组上使用 for in，索引顺序依赖于实现，可能不会按照您期望的顺序访问数组值，当顺序很重要时，最好使用 for 循环、for of 循环或 Array.forEach()。

For Of 循环
JavaScript for of 语句循环遍历可迭代对象的值，它允许您循环遍历可迭代的数据结构，例如数组、字符串、映射、节点列表等，语法：
for (variable of iterable) {
  // code block to be executed
}
variable - 对于每次迭代，下一个属性的值都会分配给变量。变量可以用 const、let 或 var 声明。
iterable - 具有可迭代属性的对象。
遍历字符串：
let language = "JavaScript";
let text = "";
for (let x of language) {
text += x + " ";                    // 返回 J a v a s c r i p t
}

While 循环
while 循环会一直循环代码块，只要指定的条件为 true，语法：
while (条件) {
    要执行的代码块
}
在下面的例子中，循环中的代码将运行，一遍又一遍，只要变量（i）小于 10：
while (i < 10) {
    text += "数字是 " + i;
    i++;
}
（注：如果您忘了对条件中使用的变量进行递增，那么循环永不会结束。这会导致浏览器崩溃。）

Do/While 循环
do/while 循环是 while 循环的变体。在检查条件是否为真之前，这种循环会执行一次代码块，然后只要条件为真就会重复循环，语法：
do {
    要执行的代码块
}
while (条件);
下面的例子使用了 do/while 循环。该循环会执行至少一次，即使条件为 false，因为代码块会在条件测试之前执行：
do {
    text += "The number is " + i;
    i++;
 }
while (i < 10);
（注：不要忘记对条件中所用变量进行递增，否则循环永不会结束！）
```

### Break 和 Continue：
```
Break 语句，它被用于“跳出” switch 语句，break 语句也可用于跳出循环，break 语句会中断循环，并继续执行循环之后的代码（如果有）：
for (i = 0; i < 10; i++) {
    if (i === 3) { break; }
    text += "数字是 " + i + " ";                // 返回 数字是 0 数字是 1 数字是 2
}
continue 语句中断（循环中）的一个迭代，如果发生指定的条件。然后继续循环中的下一个迭代，本例跳过值 3 ：
for (i = 0; i < 10; i++) {
    if (i === 3) { continue; }
    text += "数字是 " + i + "<br>";             // 返回 数字是 0 数字是 1 数字是 2 数字是 4 数字是 5 数字是 6 数字是 7 数字是 8 数字是 9
} 

JavaScript 标签，如需标记 JavaScript 语句，请将标签名和冒号置于语句之前：
label:
statements
break 和 continue 语句是仅有的可“跳出”代码块的 JavaScript 语句，语法：
break labelname;
continue labelname;
continue 语句（不论有无标签引用）只能用于跳过一个迭代。
break 语句，如果没有标签引用，只能用于跳出一个循环或一个 switch。
如果有标签引用，则 break 语句可用于跳出任意代码块：
var cars = ["BMW", "Volvo", "porsche", "Ford"];
var text = "";
list: {
  text += cars[0] + " "; 
  text += cars[1] + " "; 
  break list;                             
  text += cars[2] + " "; 
  text += cars[3] + " ";                       // 返回 BMW Volvo
}
```

### typeof:
```
在 JavaScript 中有 5 种不同的可以包含值的数据类型：
字符串（string）
数字（number）
布尔（boolean）
对象（object）
函数（function）
有三种对象类型：
对象（Object）
日期（Date）
数组（Array）
以及 2 种不能包含值的数据类型：
null
undefined

typeof 运算符,您可以使用 typeof 运算符来确定 JavaScript 变量的数据类型:
typeof "Bill"                 // 返回 "string"
typeof 3.14                   // 返回 "number"
typeof NaN                    // 返回 "number"
typeof false                  // 返回 "boolean"
typeof [1,2,3,4]              // 返回 "object"
typeof {name:'Bill', age:19}  // 返回 "object"
typeof new Date()             // 返回 "object"
typeof function () {}         // 返回 "function"
typeof myCar                  // 返回 "undefined" *
typeof null                   // 返回 "object"
(注：NaN 的数据类型是数字;数组的数据类型是对象;日期的数据类型是对象;null 的数据类型是 object;未定义变量的数据类型为 undefined *;未赋值的变量的数据类型也是 undefined *）
您无法使用 typeof 来确定 JavaScript 对象是否是数组（或日期）。

constructor 属性返回所有 JavaScript 变量的构造函数：
"Bill".constructor                // 返回 function String()  {[native code]}
(3.14).constructor                // 返回 function Number()  {[native code]}
false.constructor                 // 返回 function Boolean() {[native code]}
[1,2,3,4].constructor             // 返回 function Array()   {[native code]}
{name:'Bill',age:19}.constructor  // 返回 function Object()  {[native code]}
new Date().constructor            // 返回 function Date()    {[native code]}
function () {}.constructor        // 返回 function Function(){[native code]}
您可以检查 constructor 属性以确定对象是否为数组（包含 "Array" 一词）：
function isArray(myArray) {
  return myArray.constructor.toString().indexOf("Array") > -1;
}
您也可以检查 constructor 属性以确定对象是否为日期（包含 "Date" 一词）：
function isDate(myDate) {
  return myDate.constructor.toString().indexOf("Date") > -1;
}
```

### 位运算符：
```
JavaScript 位运算符
运算符	              名称	            描述
&	               AND	           当对一对数位执行位运算 AND 时，如果数位均为 1 则返回 1
|	               OR	           当对一对数位执行位运算 OR 时，如果其中一位是 1 则返回 1
^	               XOR	           当对一对数位进行位运算 XOR 时，如果数位是不同的则返回 1
~	               NOT	           反转所有位
<<	             零填充左位移	   通过从右推入零向左位移，并使最左边的位脱落。
>>	             有符号右位移	   通过从左推入最左位的拷贝来向右位移，并使最右边的位脱落。
>>>	             零填充右位移	   通过从左推入零来向右位移，并使最右边的位脱落。

JavaScript 使用 32 位按位运算数，JavaScript 将数字存储为 64 位浮点数，但所有按位运算都以 32 位二进制数执行，在执行位运算之前，JavaScript 将数字转换为 32 位有符号整数，执行按位操作后，结果将转换回 64 位 JavaScript 数，由于 JavaScript 使用 32 位有符号整数，所以JavaScript 会将~5返回 -6：
00000000000000000000000000000101 (5)
11111111111111111111111111111010 (~5 = -6)
有符号整数使用最左边的位作为减号。

JavaScript（零填充）位运算左移（<<）
这是零填充的左移。一个或多个零数位从右被推入，最左侧的数位被移除：
十进制	           二进制
5	          00000000000000000000000000000101
5 << 1	          00000000000000000000000000001010 (10)

JavaScript（有符号）位运算右移（>>）
这是保留符号的右移。最左侧的数位被从左侧推入，最右侧的数位被移出：
十进制	          二进制
-5	         11111111111111111111111111111011
-5 >> 1	         11111111111111111111111111111101 (-3)

JavaScript（零填充）右移（>>>）
这是零填充的右移。一个或多个零数位从左侧被推入，最右侧的数位被移出：
十进制	         二进制
5	        00000000000000000000000000000101
5 >>> 1	        00000000000000000000000000000010 (2)
```

### 正则表达式：
```
正则表达式是构成搜索模式（search pattern）的字符序列，当您搜索文本中的数据时，您可使用搜索模式来描述您搜索的内容，正则表达式可以是单字符，或者更复杂的模式，正则表达式可用于执行所有类型的文本搜索和文本替换操作，语法：
/pattern/modifiers;                // pattern 是模式（在搜索中使用）；modifiers 是修饰符。

使用字符串方法
在 JavaScript 中，正则表达式常用于两个字符串方法：search() 和 replace()。
search() 方法使用表达式来搜索匹配，然后返回匹配的位置，使用正则表达式执行搜索字符串中 "w3school" 的大小写不敏感的搜索：
var str = "Visit W3School";
var n = str.search(/w3school/i);                 // 返回 n 的值为 6
replace() 方法返回模式被替换处修改后的字符串，使用大小写不明的正则表达式以 W3school 来替换字符串中的 Microsoft：
var str = "Visit Microsoft!";
var res = str.replace(/microsoft/i, "W3School");       // 返回 res 的值为 Visit W3School!

正则表达式修饰符
修饰符可用于大小写不敏感的更全局的搜素：
修饰符	                  描述	
i	                 执行对大小写不敏感的匹配。	
g	                 执行全局匹配（查找所有匹配而非在找到第一个匹配后停止）。	
m	                 执行多行匹配。	

正则表达式模式
括号用于查找一定范围的字符串：
表达式	        描述	
[abc]	       查找方括号之间的任何字符。	
[0-9]	       查找任何从 0 至 9 的数字。	
(x|y)	       查找由 | 分隔的任何选项。

元字符（Metacharacter）是拥有特殊含义的字符：
元字符	        描述
\d	       查找数字。	
\s	       查找空白字符。	
\b	       匹配单词边界。	
\uxxxx	       查找以十六进制数 xxxx 规定的 Unicode 字符。	

Quantifiers 定义量词：
量词	 描述	
n+	  匹配任何包含至少一个 n 的字符串。	
n*	  匹配任何包含零个或多个 n 的字符串。	
n?	  匹配任何包含零个或一个 n 的字符串。	

正则式方法
test() 是一个正则表达式方法,它通过模式来搜索字符串，然后根据结果返回 true 或 false,下面的例子搜索字符串中的字符 "e"：
/e/.test("The best things in life are free!");             // 返回 true
exec() 方法是一个正则表达式方法，它通过指定的模式（pattern）搜索字符串，并返回已找到的文本，如果未找到匹配，则返回 null，下面的例子搜索字符串中的字符 "e"：
/e/.exec("The best things in life are free!");             // 返回 e
```

### 错误：
```
try 语句使您能够测试代码块中的错误。
catch 语句允许您处理错误。
throw 语句允许您创建自定义错误。
finally 使您能够执行代码，在 try 和 catch 之后，无论结果如何。

JavaScript try 和 catch
try 语句允许您定义一个代码块，以便在执行时检测错误，catch 语句允许你定义一个要执行的代码块，如果 try 代码块中发生错误，JavaScript 语句 try 和 catch 成对出现：
try {
     供测试的代码块
}
 catch(err) {
     处理错误的代码块
} 

throw 语句
throw 语句允许您创建自定义错误，从技术上讲您能够抛出异常（抛出错误），异常可以是 JavaScript 字符串、数字、布尔或对象。
本例会检查输入。如果值是错误的，将抛出异常（err），该异常（err）被 catch 语句捕获并显示一条自定义的错误消息：
<!DOCTYPE html>
<html>
<body>
<p>请输入 5 - 10 之间的数字：</p>
<input id="demo" type="text">
<button type="button" onclick="myFunction()">测试输入</button>
<p id="message"></p>
<script>
function myFunction() {
    var message, x;
    message = document.getElementById("message");
    message.innerHTML = "";
    x = document.getElementById("demo").value;
    try { 
        if(x == "") throw "空的";
         if(isNaN(x)) throw "不是数字";
         x = Number(x);
        if(x < 5) throw  "太小";
        if(x > 10) throw "太大";
    }
    catch(err) {
        message.innerHTML = "输入是 " + err;
    }
}
</script>
</body>
</html> 

finally 语句
finally 语句允许您在 try 和 catch 之后执行代码，无论结果：
try {
     // 供测试的代码块
}
 catch(err) {
     // 处理错误的代码块
} 
finally {
     // 无论结果如何都执行的代码块
}

Error 对象
JavaScript 拥有当错误发生时提供错误信息的内置 error 对象，error 对象提供两个有用的属性：name 和 message。
Error 对象属性
属性	     描述
name	    设置或返回错误名
message	    设置或返回错误消息（一条字符串）

Error Name Values
error 的 name 属性可返回六个不同的值：
错误名	            描述
EvalError	    已在 eval() 函数中发生的错误
RangeError	    已发生超出数字范围的错误（范围错误）
ReferenceError	    已发生非法引用（引用错误）
SyntaxError	    已发生语法错误（语法错误）
TypeError	    已发生类型错误（类型错误）
URIError	    在 encodeURI() 中已发生的错误（URI错误）
```

### Hoisting：
```
提升（Hoisting）是 JavaScript 将声明移至顶部的默认行为。
在 JavaScript 中，可以在使用变量之后对其进行声明，换句话说，可以在声明变量之前使用它：
x = 5;                                  // 把 5 赋值给 x
elem = document.getElementById("demo"); // 查找元素
elem.innerHTML = x;                     // 在元素中显示 x
var x;                                  // 声明 x

let 和 const 关键字，用 let 或 const 声明的变量和常量不会被提升！
JavaScript 初始化也不会被提升，JavaScript 只提升声明，而非初始化。
```

### 严格模式：
```
"use strict"; 定义 JavaScript 代码应该以“严格模式”执行，"use strict" 是 JavaScript 1.8.5 中的新指令（ECMAScript version 5），"use strict"; 的作用是指示 JavaScript 代码应该以“严格模式”执行。
声明严格模式，通过在脚本或函数的开头添加 "use strict"; 来声明严格模式，在脚本开头进行声明，拥有全局作用域（脚本中的所有代码均以严格模式来执行）；在函数中声明严格模式，拥有局部作用域。（只有函数中的代码以严格模式执行）
严格模式中不允许的事项
在不声明变量或对象的情况下使用变量，是不允许的：
"use strict";
x = 3.14;                // 这将引发错误
x = {p1:10, p2:20};      // 这将引发错误
删除变量（或对象）是不允许的：
"use strict";
var x = 3.14;
delete x;                // 这将引发错误
删除函数是不允许的：
"use strict";
function x(p1, p2) {}; 
delete x;                 // 这将引发错误
重复参数名是不允许的：
"use strict";
function x(p1, p1) {};   // 这将引发错误
八进制数值文本是不允许的：
"use strict";
var x = 010;             // 这将引发错误
转义字符是不允许的：
"use strict";
var x = \010;            // 这将引发错误
写入只读属性是不允许的：
"use strict";
var obj = {};
Object.defineProperty(obj, "x", {value:0, writable:false});
obj.x = 3.14;            // 这将引发错误
写入只能获取的属性是不允许的：
"use strict";
var obj = {get x() {return 0} };
obj.x = 3.14;            // 这将引发错误
删除不可删除的属性是不允许的：
"use strict";
delete Object.prototype; // 这将引发错误
字符串 "eval" 和字符串 "arguments" 不可用作变量：
"use strict";
var eval = 3.14;         // 这将引发错误
var arguments = 3.14;    // 这将引发错误
with 语句是不允许的：
"use strict";
with (Math){x = cos(2)}; // 这将引发错误
处于安全考虑，不允许 eval() 在其被调用的作用域中创建变量：
"use strict";
eval ("var x = 2");
alert (x);               // 这将引发错误
严格模式中不允许使用为未来预留的关键词。它们是：
implements；interface；let；package；private；protected；public；static；yield
"use strict";
var public = 1500;      // 这将引发错误
提示：在类似 f() 的函数调用中，this 的值是全局对象。在严格模式中，现在它成为了 undefined。（注："use strict" 指令只能在脚本或函数的开头被识别。）
```

### this 关键词：
```
JavaScript this 关键词指的是它所属的对象，它拥有不同的值，具体取决于它的使用位置：
在方法中，this 指的是所有者对象。         // 方法（method）是通过对象调用的javascript函数，当将函数和对象和写在一起时，函数（function）就变成了方法（method）。 
单独的情况下，this 指的是全局对象。
在函数中，this 指的是全局对象。
在函数中，严格模式下，this 是 undefined。
在事件中，this 指的是接收事件的元素。
像 call() 和 apply() 这样的方法可以将 this 引用到任何对象。

单独的 this
在单独使用时，拥有者是全局对象，因此 this 指的是全局对象。在浏览器窗口中，全局对象是 [object Window]：
var x = this;         // x 返回 [object Window]
在严格模式中，如果单独使用，那么 this 指的是全局对象 [object Window]：
"use strict";
var x = this;         // x 返回 [object Window]

函数中的 this（默认）
在 JavaScript 函数中，函数的拥有者默认绑定 this。因此，在函数中，this 指的是全局对象 [object Window]： 
function myFunction() {return this;}              // myFunction() 返回 [object Window]
JavaScript 严格模式不允许默认绑定。因此，在函数中使用时，在严格模式下，this 是未定义的（undefined）：
"use strict";
function myFunction() {return this;}              // myFunction() 返回 undefined


事件处理程序中的 this,在 HTML 事件处理程序中，this 指的是接收此事件的 HTML 元素：
<button onclick="this.style.display='none'">点击来删除我！</button>      // 点击按钮后改变了元素的属性，按钮便会消失

显式函数绑定
call() 和 apply() 方法是预定义的 JavaScript 方法。它们都可以用于将另一个对象作为参数调用对象方法：
var person1 = {
  fullName: function() {
    return this.firstName + " " + this.lastName;
  }
}
var person2 = {
  firstName:"Bill",
  lastName: "Gates",
}
var x = person1.fullName.call(person2);          // x 会返回 Bill Gates
```

### 箭头函数：
```
ES6 中引入了箭头函数，箭头函数允许我们编写更短的函数。
之前：
hello = function() {return "Hello World!";}
用了箭头函数之后：
hello = () => {return "Hello World!";}
如果函数只有一个语句，并且该语句返回一个值，则可以去掉括号和 return 关键字：
hello = () => "Hello World!";
（注：这仅在函数只有一条语句时才有效。）
如果您有参数，则将它们传递到括号内：
hello = (val) => "Hello " + val;
事实上，如果只有一个参数，您也可以略过括号：
hello = val => "Hello " + val;

与常规函数相比，箭头函数对 this 的处理也有所不同。
简而言之，使用箭头函数没有对 this 的绑定。在常规函数中，关键字 this 表示调用该函数的对象，可以是窗口、文档、按钮或其他任何东西。对于箭头函数，this 关键字始终表示定义箭头函数的对象。
```

### 类：
```
JavaScript 类是 JavaScript 对象的模板，语法：
class ClassName {constructor() { ... }}
请使用关键字 class 创建类，请始终添加名为 constructor() 的方法。
下面的例子创建了一个名为 "Car" 的类，该类有两个初始属性："name" 和 "year"，JavaScript 类不是对象，它只是 JavaScript 对象的模板：
class Car {
  constructor(name, year) {
    this.name = name;
    this.year = year;
  }
}
如果您有一个类，那么您可以使用该类来创建对象，下面的例子使用 Car 类创建了两个 Car 对象，在创建新对象时会自动调用 constructor 方法：
let myCar1 = new Car("Ford", 2014);
let myCar2 = new Car("Audi", 2019);

Constructor 方法
构造方法是一种特殊的方法：
它必须拥有确切名称的“构造函数”
创建新对象时自动执行
用于初始化对象属性
如果未定义构造函数方法，JavaScript 会添加空的构造函数方法。

Class 方法
类方法的创建，语法：
class ClassName {
  constructor() { ... }
  method_1() { ... }
  method_2() { ... }
  method_3() { ... }
}
与对象方法相同，请使用关键字 class 创建类，请始终添加 constructor() 方法，然后添加任意数量的方法。
```

### JSON:
```
JSON 是存储和传输数据的格式，JSON 经常在数据从服务器发送到网页时使用，JSON 语法规则：
数据是名称/值对
数据由逗号分隔
花括号保存对象
方括号保存数组

JSON 数据 - 名称和值
JSON 数据的书写方式是名称/值对，类似 JavaScript 对象属性。名称/值对由（双引号中的）字段名构成，其后是冒号，再其后是值：
"firstName":"Bill"
（注：JSON 名称需要双引号。JavaScript 名称不需要。）
JSON 对象
JSON 对象是在花括号内书写的，类似 JavaScript，对象能够包含多个名称/值对：
{"firstName":"Bill", "lastName":"Gates"} 
JSON 数组
JSON 数组在方括号中书写，类似 JavaScript，数组能够包含对象：
"employees":[
    {"firstName":"Bill", "lastName":"Gates"}, 
    {"firstName":"Steve", "lastName":"Jobs"}, 
    {"firstName":"Alan", "lastName":"Turing"}
]
在上面的例子中，对象 "employees" 是一个数组。它包含了三个对象。每个对象代表一个人的一条记录（带有名和姓）。

把 JSON 文本转换为 JavaScript 对象
JSON 的通常用法是从 web 服务器读取数据，然后在网页中显示数据，为了简单起见，可以使用字符串作为输入演示，首先，创建包含 JSON 语法的 JavaScript 字符串：
var text = '{ "employees" : [' +
'{ "firstName":"Bill" , "lastName":"Gates" },' +
'{ "firstName":"Steve" , "lastName":"Jobs" },' +
'{ "firstName":"Alan" , "lastName":"Turing" } ]}';
然后，使用 JavaScript 的内建函数 JSON.parse() 来把这个字符串转换为 JavaScript 对象：
var obj = JSON.parse(text);
最后，请在您的页面中使用这个新的 JavaScript 对象：
<p id="demo"></p>
<script>
document.getElementById("demo").innerHTML =
obj.employees[1].firstName + " " + obj.employees[1].lastName;
</script> 
```

### 调试：
```
错误总会发生，每当您写一些新的计算机代码时。
console.log() 方法，如果您的浏览器支持调试，那么您可以使用 console.log() 在调试窗口中显示 JavaScript 的值。
debugger 关键词会停止 JavaScript 的执行，并调用（如果有）调试函数，这与在调试器中设置断点的功能是一样的。
```

### 对象定义：
```
在 JavaScript 中，对象是王。如果您理解了对象，就理解了 JavaScript。在 JavaScript 中，几乎“所有事物”都是对象：
布尔是对象（如果用 new 关键词定义）
数字是对象（如果用 new 关键词定义）
字符串是对象（如果用 new 关键词定义）
日期永远都是对象
算术永远都是对象
正则表达式永远都是对象
数组永远都是对象
函数永远都是对象
对象永远都是对象
所有 JavaScript 值，除了原始值，都是对象。

JavaScript 原始值
原始值指的是没有属性或方法的值，原始数据类型指的是拥有原始值的数据。
JavaScript 定义了 5 种原始数据类型：
string
number
boolean
null
undefined
原始值是一成不变的（它们是硬编码的，因此不能改变）。

创建 JavaScript 对象
通过 JavaScript，您能够定义和创建自己的对象，有不同的方法来创建对象：
定义和创建单个对象，使用对象文字。
定义和创建单个对象，通过关键词 new。
定义对象构造器，然后创建构造类型的对象。
在 ECMAScript 5 中，也可以通过函数 Object.create() 来创建对象。
使用对象字面量
这是创建对象最简答的方法，使用对象文字，您可以在一条语句中定义和创建对象，对象文字指的是花括号 {} 中的名称:值对（比如 age:62），下面的例子创建带有四个属性的新的 JavaScript 对象：
var person = {firstName:"Bill", lastName:"Gates", age:62, eyeColor:"blue"};
使用 JavaScript 关键词 new
下面的例子也创建了带有四个属性的新的 JavaScript 对象：
var person = new Object();
person.firstName = "Bill";
person.lastName = "Gates";
person.age = 50;
person.eyeColor = "blue"; 
（注：出于简易性、可读性和执行速度的考虑，请使用第一种创建方法（对象文字方法））
JavaScript 对象是易变的
对象是易变的：它们通过引用来寻址，而非值，如果 person 是一个对象，下面的语句不会创建 person 的副本：
var x = person;  // 这不会创建 person 的副本。
对象 x 并非 person 的副本。它就是 person。x 和 person 是同一个对象，对 x 的任何改变都将改变 person，因为 x 和 person 是相同的对象。
(注：JavaScript 变量不是易变的。只有 JavaScript 对象如此)
```

### 对象属性：
```
访问对象属性的语法是：
objectName.property           // person.age
或者：
objectName["property"]       // person["age"]
或者：
objectName[expression]       // x = "age"; person[x]

删除属性
delete 关键词从对象中删除属性：
var person = {firstName:"Bill", lastName:"Gates", age:62, eyeColor:"blue"};
delete person.age;   // 或 delete person["age"];
（注：delete 关键词会同时删除属性的值和属性本身。删除完成后，属性在被添加回来之前是无法使用的。delete 操作符被设计用于对象属性。它对变量或函数没有影响。delete 操作符不应被用于预定义的 JavaScript 对象属性。这样做会使应用程序崩溃。）
```

### 对象方法：
```
访问对象方法,请使用如下语法创建对象方法：
methodName : function() { 代码行 }
请通过如下语法来访问对象方法：
objectName.methodName()
您通常会把 fullName() 描述为 person 对象的方法，把 fullName 描述为属性。fullName 属性在被通过 () 调用后会以函数形式执行。如果您访问 fullName 属性时没有使用 ()，则将返回函数定义。
```

### 对象显示：
```
显示 JavaScript 对象的一些常见解决方案是：
按名称显示对象属性
循环显示对象属性
使用 Object.values() 显示对象
使用 JSON.stringify() 显示对象

在循环中显示对象
可以在循环中收集对象的属性：
for (let x in person) {
txt += person[x] + " ";
};
（注：您必须在循环中使用 person[x]。person.x 将不起作用（因为 x 是一个变量）。）


使用 Object.values()
通过使用 Object.values()，任何 JavaScript 对象都可以被转换为数组：
const person = {
  name: "Bill",
  age: 19,
  city: "Seattle"
};
const myArray = Object.values(person);          // myArray 返回 Bill,19,Seattle

使用 JSON.stringify()
任何 JavaScript 对象都可以使用 JavaScript 函数 JSON.stringify() 进行字符串化（转换为字符串）：
const person = {
  name: "Bill",
  age: 19,
  city: "Seattle"
};
let myString = JSON.stringify(person);          // myString 返回 {"name":"Bill","age":19,"city":"Seattle"}
```

### 对象访问器：
```
JavaScript 访问器（Getter 和 Setter），ECMAScript 5 (2009) 引入了 Getter 和 Setter，Getter 和 Setter 允许您定义对象访问器（被计算的属性）。

JavaScript Getter（get 关键词）
本例使用 lang 属性来获取 language 属性的值。
// 创建对象：
var person = {
  firstName: "Bill",
  lastName : "Gates",
  language : "en",
  get lang() {
    return this.language;
  }
};
// 使用 getter 来显示来自对象的数据：
document.getElementById("demo").innerHTML = person.lang;             // person.lang 返回 en

JavaScript Setter（set 关键词）
本例使用 lang 属性来设置 language 属性的值。
var person = {
  firstName: "Bill",
  lastName : "Gates",
  language : "",
  set lang(lang) {
    this.language = lang;
  }
};
// 使用 setter 来设置对象属性：
person.lang = "en";
// 显示来自对象的数据：
document.getElementById("demo").innerHTML = person.language;         // person.language 返回 en

为什么使用 Getter 和 Setter？
它提供了更简洁的语法
它允许属性和方法的语法相同
它可以确保更好的数据质量
有利于后台工作
```

### 对象构造器：
```
用大写首字母对构造器函数命名是个好习惯：
function Person(first, last, age, eye) {
    this.firstName = first;
    this.lastName = last;
    this.age = age;
    this.eyeColor = eye;
}
有时我们需要创建相同“类型”的许多对象的“蓝图”，创建一种“对象类型”的方法，是使用对象构造器函数，在上面的例子中，函数 Person() 就是对象构造器函数，通过 new 关键词调用构造器函数可以创建相同类型的对象：
var myFather = new Person("Bill", "Gates", 62, "blue");
var myMother = new Person("Steve", "Jobs", 56, "green");

为构造器添加属性
与向已有对象添加新属性不同，您无法为对象构造器添加新属性：
Person.nationality = "English";
如需向构造器添加一个新属性，您必须添加到构造器函数：
function Person(first, last, age, eyecolor) {
    this.firstName = first;
    this.lastName = last;
    this.age = age;
    this.eyeColor = eyecolor;
    this.nationality = "English";
}
提示：为构造器添加方法也是如此。
```

### 对象原型：
```
原型继承
所有 JavaScript 对象都从原型继承属性和方法。日期对象继承自 Date.prototype。数组对象继承自 Array.prototype。Person 对象继承自 Person.prototype。
Object.prototype 位于原型继承链的顶端：日期对象、数组对象和 Person 对象都继承自 Object.prototype。

使用 prototype 属性
JavaScript prototype 属性允许您为对象构造器添加新属性：
function Person(first, last, age, eyecolor) {
    this.firstName = first;
    this.lastName = last;
    this.age = age;
    this.eyeColor = eyecolor;
}
Person.prototype.nationality = "English";
提示：JavaScript prototype 属性也允许您为对象构造器添加新方法。（注：请只修改您自己的原型。绝不要修改标准 JavaScript 对象的原型。）
```

### ES 对象方法：
```
ECMAScript 5 (2009) 向 JavaScript 添加了许多新的对象方法。
管理对象
// 以现有对象为原型创建对象
Object.create()
// 添加或更改对象属性
Object.defineProperty(object, property, descriptor)
// 添加或更改对象属性
Object.defineProperties(object, descriptors)
// 访问属性
Object.getOwnPropertyDescriptor(object, property)
// 以数组返回所有属性
Object.getOwnPropertyNames(object)
// 访问原型
Object.getPrototypeOf(object)
// 以数组返回可枚举属性
Object.keys(object)
保护对象
// 防止向对象添加属性
Object.preventExtensions(object)
// 如果属性可以添加到对象，则返回 true
Object.isExtensible(object)
// 防止更改对象属性（不是值）
Object.seal(object)
// 如果对象被密封，则返回 true
Object.isSealed(object)
// 防止对对象进行任何更改
Object.freeze(object)
// 如果对象被冻结，则返回 true
Object.isFrozen(object)

Object.defineProperty() 方法会直接在一个对象上定义一个新属性，或者修改一个对象的现有属性，并返回此对象。语法：
Object.defineProperty(obj, prop, descriptor)
obj，要定义属性的对象；prop，要定义或修改的属性的名称或 Symbol ；descriptor，要定义或修改的属性描述符。

更改元数据
ES5 允许更改以下属性元数据：
writable : true/false      // 属性值可更改
enumerable : true/false    // 属性可枚举
configurable : true/false  // 属性可重新配置

ES5 允许更改 getter 和 setter：
// 定义 getter
get: function() { return language }
// 定义 setter
set: function(value) { language = value }
```

### Map 对象：
```
Map 对象存有键值对，其中的键可以是任何数据类型，Map 对象记得键的原始插入顺序，Map 对象具有表示映射大小的属性。
基本的 Map() 方法
方法	              描述
new Map()	     创建新的 Map 对象。
set()	             为 Map 对象中的键设置值。
get()	             获取 Map 对象中键的值。
entries()	     返回 Map 对象中键/值对的数组。
keys()	             返回 Map 对象中键的数组。
values()	     返回 Map 对象中值的数组。

创建 Map 对象
// 创建对象
const apples = {name: 'Apples'};
const bananas = {name: 'Bananas'};
const oranges = {name: 'Oranges'};
// 创建新的 Map
const fruits = new Map();
// 向 Map 添加新元素
fruits.set(apples, 500);
fruits.set(bananas, 300);
fruits.set(oranges, 200);
获取键的值
get() 方法获取 Map 中键的值：
fruits.get(apples);    // 返回 500
fruits.get("apples");  // 返回 undefined
（注：键是一个对象，而不是一个字符串）

其他 Map() 方法
方法	              描述
clear()	            删除 Map 中的所有元素。
delete()	    删除由键指定的元素。
has()	            如果键存在，则返回 true。
forEach()	    为每个键/值对调用回调。
Map() 属性
属性	 描述
size	获取 Map 中键的值。

Map.size 返回 Map 中元素的数量：
fruits.size;
Map.delete() 删除 Map 元素：
fruits.delete(apples);
Map.clear() 从 Map 中移除所有元素：
fruits.clear();
如果 Map 中存在键，则 Map.has() 返回 true：
fruits.has(apples);

JavaScript 对象和 Map 之间的差异：
            对象	                            Map
Size	   对象没有 size 属性	                 Maps 有 size 属性
键类型	   对象键必须是字符串（或符号）	         Map 键可以是任何数据类型
键顺序	   对象键没有很好地排序	                 Map 键按插入排序
默认	   对象有默认键	                         Map 没有默认键
```

### set 对象：
```
Set 是唯一值的集合。每个值在 Set 中只能出现一次。一个 Set 可以容纳任何数据类型的任何值。
创建一个 Set 并添加现有变量：
// 创建新的变量
const a = "a";
const b = "b";
const c = "c";
// 创建 Set
const letters = new Set();
// Add the values to the Set
letters.add(a);
letters.add(b);
letters.add(c);

Set 对象的方法和属性
new Set()	        创建新的 Set 对象。
add()	                向 Set 添加新元素。
clear()	                从 Set 中删除所有元素。
delete()	        删除由其值指定的元素。
entries()	        返回 Set 对象中值的数组。
has()	                如果值存在则返回 true。
forEach()	        为每个元素调用回调。
keys()	                返回 Set 对象中值的数组。
values()	        与 keys() 相同。
size	                返回元素计数。
```

### 函数定义：
```
JavaScript 函数是通过 function 关键词定义的。您可以使用函数声明或函数表达式。定义为对象属性的函数，被称为对象的方法。方法也是函数，只是比较特殊的函数。 
函数表达式，JavaScript 函数可以使用表达式来定义。
函数表达式可以在变量中存储，在变量中保存函数表达式之后，此变量可用作函数：
var x = function (a, b) {return a * b};
var z = x(4, 3);
上面的函数实际上是一个匿名函数（没有名称的函数）。存放在变量中的函数不需要函数名。他们总是使用变量名调用。上面的函数使用分号结尾，因为它是可执行语句的一部分。

Function() 构造器
正如您在之前的例子中看到的，JavaScript 函数是通过 function 关键词定义的。函数也可以通过名为 Function() 的内建 JavaScript 函数构造器来定义：
var myFunction = new Function("a", "b", "return a * b");
var x = myFunction(4, 3);
您实际上无需使用函数构造器。上面的例子这么写也是一样的：
var myFunction = function (a, b) {return a * b};
var x = myFunction(4, 3);
大多数情况下，您可以避免在 JavaScript 中使用 new 关键词。

自调用函数
函数表达式可以作为“自调用”。自调用表达式是自动被调用（开始）的，在不进行调用的情况下。函数表达式会自动执行，假如表达式后面跟着 ()。您无法对函数声明进行自调用。您需要在函数周围添加括号，以指示它是一个函数表达式：
(function () {
    var x = "Hello!!";      // 我会调用我自己
})();
```

### 函数参数：
```
JavaScript 函数不会对参数值进行任何检查。
arguments 对象
JavaScript 函数有一个名为 arguments 对象的内置对象。arguments 对象包含函数调用时使用的参数数组。这样，您就可以简单地使用函数来查找（例如）数字列表中的最高值：
x = findMax(1, 123, 500, 115, 44, 88);
function findMax() {
    var i;
    var max = -Infinity;
    for (i = 0; i < arguments.length; i++) {
        if (arguments[i] > max) {
            max = arguments[i];
        }
    }
    return max;
}
或创建一个函数来总和所有输入值：
x = sumAll(1, 123, 500, 115, 44, 88);
function sumAll() {
    var i, sum = 0;
    for (i = 0; i < arguments.length; i++) {
        sum += arguments[i];
    }
    return sum;
}
```

### 函数调用：
```
JavaScript 函数内部的代码会在“某物”调用它时执行。
全局对象
当不带拥有者对象调用对象时，this 的值成为全局对象。在 web 浏览器中，全局对象就是浏览器对象。本例以 this 的值返回这个 window 对象：
var x = myFunction();            // x 返回 [object Window]
function myFunction() {
   return this;
}
调用一个函数作为一个全局函数，会导致 this 的值成为全局对象。作为变量来使用 window 对象很容易使程序崩溃。

作为方法来调用函数
fullName 方法是一个函数。该函数属于对象。myObject 是函数的拥有者。被称为 this 的事物，是“拥有”这段 JavaScript 代码的对象。在此例中，this 的值是 myObject：
var myObject = {
    firstName:"Bill",
    lastName: "Gates",
    fullName: function () {
        return this;
    }
}
myObject.fullName();          // 将返回 [object Object]
以对象方法来调用函数，会导致 this 的值成为对象本身。

通过函数构造器来调用函数
如果函数调用的前面是 new 关键字，那么这是一个构造函数调用。它看起来像你创建一个新的函数，但由于 JavaScript 函数是对象，你实际上创建一个新对象：
// 这是函数构造器：
function myFunction(arg1, arg2) {
    this.firstName = arg1;
    this.lastName  = arg2;
}
// 创建了一个新对象：
var x = new myFunction("Bill", "Gates");
x.firstName;                             // 会返回 "Bill"
构造器调用会创建新对象。新对象会从其构造器继承属性和方法。构造器内的 this 关键词没有值。this 的值会成为调用函数时创建的新对象。

函数 Call:
使用 call() 方法，您可以编写能够在不同对象上使用的方法。call() 方法是预定义的 JavaScript 方法。它可以用来调用所有者对象作为参数的方法。通过 call()，您能够使用属于另一个对象的方法。通过 call()，您能够使用属于另一个对象的方法。本例调用 person 的 fullName 方法，并用于 person1：
var person = {
    fullName: function() {
        return this.firstName + " " + this.lastName;
    }
}
var person1 = {
    firstName:"Bill",
    lastName: "Gates",
}
person.fullName.call(person1);  // 将返回 "Bill Gates"

call() 方法可接受参数：
var person = {
  fullName: function(city, country) {
    return this.firstName + " " + this.lastName + "," + city + "," + country;
  }
}
var person1 = {
  firstName:"Bill",
  lastName: "Gates"
}
person.fullName.call(person1, "Seattle", "USA");
```

### 函数 Apply:
```
call() 和 apply() 之间的区别
不同之处是：
call() 方法分别接受参数。
apply() 方法接受数组形式的参数。
如果要使用数组而不是参数列表，则 apply() 方法非常方便。

apply() 方法接受数组中的参数：
var person = {
  fullName: function(city, country) {
    return this.firstName + " " + this.lastName + "," + city + "," + country;
  }
}
var person1 = {
  firstName:"Bill",
  lastName: "Gates"
}
person.fullName.apply(person1, ["Oslo", "Norway"]);

在数组上模拟 max 方法
您可以使用 Math.max() 方法找到（数字列表中的）最大数字：
Math.max(1,2,3);  // 会返回 3
由于 JavaScript 数组没有 max() 方法，因此您可以应用 Math.max() 方法:
Math.max.apply(null, [1,2,3]); // 也会返回 3
第一个参数（null）无关紧要。在本例中未使用它。这些例子会给出相同的结果：
Math.max.apply(Math, [1,2,3]); // 也会返回 3
Math.max.apply(" ", [1,2,3]); // 也会返回 3
Math.max.apply(0, [1,2,3]); // 也会返回 3
(注：在 JavaScript 严格模式下，如果 apply() 方法的第一个参数不是对象，则它将成为被调用函数的所有者（对象）。在“非严格”模式下，它成为全局对象。)
```

### 闭包：
```
JavaScript 变量属于本地或全局作用域。
全局变量能够通过闭包实现局部（私有）。

1、函数自调用方法
(function () {
	altert("页面一加载自动调用")；
})();
2、闭包，函数内的参数数据外部不可以访问，通过返回子函数操作闭包中的数据
//页面一加载初始化counter = 0;
var add=(function () {
    var counter = 0;
    return function () {return counter += 1;}
})();
//参数add返回一个无参数的子函数
//add()实际调用的是function () {return counter += 1;}无参数子函数
//通过调用闭包中无参数的子函数修改闭包中的数据，保证闭包中的数据不让外部修改
add();//1
add();//2
add();//3
这被称为 JavaScript 闭包。它使函数拥有“私有”变量成为可能。计数器被这个匿名函数的作用域保护，并且只能使用 add 函数来修改。闭包指的是有权访问父作用域的函数，即使在父函数关闭之后。
```

### 类继承：
```
构造方法，构造方法是一种特殊的方法：
它必须有确切的名称的 “constructor”
创建新对象时自动执行
用于初始化对象属性
如果您没有定义构造方法，JavaScript 会添加一个空的构造方法。

类继承，如需创建类继承，请使用 extends 关键字，使用类继承创建的类继承了另一个类的所有方法：
class Car {
  constructor(brand) {
    this.carname = brand;
  }
  present() {
    return 'I have a ' + this.carname;
  }
}
class Model extends Car {
  constructor(brand, mod) {
    super(brand);
    this.model = mod;
  }
  show() {
    return this.present() + ', it is a ' + this.model;
  }
}
let myCar = new Model("Ford", "Mustang");
document.getElementById("demo").innerHTML = myCar.show();            // 返回 I have a Ford, it is a Mustang
super() 方法引用父类。
通过在 constructor 方法中调用 super() 方法，我们调用了父级的 constructor 方法，获得了父级的属性和方法的访问权限。继承对于代码可重用性很有用：在创建新类时重用现有类的属性和方法。

Getter 和 Setter
类还允许您使用 getter 和 setter。为您的属性使用 getter 和 setter 很聪明，特别是如果您想在返回它们之前或在设置它们之前对值做一些特殊的事情。如需在类中添加 getter 和 setter，请使用 get 和 set 关键字：
class Car {
  constructor(brand) {
    this._carname = brand;
  }
  get carname() {
    return this._carname;
  }
  set carname(x) {
    this._carname = x;
  }
}
let myCar = new Car("Ford");
document.getElementById("demo").innerHTML = myCar.carname;
（注释：即使 getter 是一个方法，当你想要获取属性值时也不要使用括号。getter/setter 方法的名称不能与属性名称相同，在本例中为 carname。许多程序员在属性名称前使用下划线字符 _ 将 getter/setter 与实际属性分开）

Hoisting
与函数和其他 JavaScript 声明不同，类声明不会被提升。这意味着您必须先声明类，然后才能使用它。
```

### Static 方法：
```
static 类方法是在类本身上定义的。您不能在对象上调用 static 方法，只能在对象类上调用：
class Car {
  constructor(name) {
    this.name = name;
  }
  static hello() {
    return "Hello!!";
  }
}
let myCar = new Car("Ford");
// 您可以在 Car 类上调用 'hello()' ：
document.getElementById("demo").innerHTML = Car.hello();
// 但不能在 Car 对象上调用：
// document.getElementById("demo").innerHTML = myCar.hello();
// 此举将引发错误。

如果要在 static 方法中使用 myCar 对象，可以将其作为参数发送：
class Car {
  constructor(name) {
    this.name = name;
  }
  static hello(x) {
    return "Hello " + x.name;
  }
}
let myCar = new Car("Ford");
document.getElementById("demo").innerHTML = Car.hello(myCar);
```

### 回调：
```
回调 (callback) 是作为参数传递给另一个函数的函数，这种技术允许函数调用另一个函数，回调函数可以在另一个函数完成后运行使用回调，您可以通过回调调用计算器函数（myCalculator），并在计算完成后让计算器函数运行回调：
function myDisplayer(some) {
  document.getElementById("demo").innerHTML = some;
}
function myCalculator(num1, num2, myCallback) {
  let sum = num1 + num2;
  myCallback(sum);
}
myCalculator(5, 5, myDisplayer);
在上面的例子中， myDisplayer 是函数的名称。它作为参数传递给 myCalculator()。当您将函数作为参数传递时，请记住不要使用括号。
正确：myCalculator(5, 5, myDisplayer);错误：myCalculator(5, 5, myDisplayer());
```

### 异步：
```
与其他函数并行运行的函数称为异步（asynchronous），一个很好的例子是 JavaScript setTimeout()：
setTimeout(myFunction, 3000);
function myFunction() {
  document.getElementById("demo").innerHTML = "I love You !!";
}
在上面等待超时的示例中，myFunction 被用作回调。函数（函数名）作为参数传递给 setTimeout()。3000 是超时前的毫秒数，所以 3 秒后会调用 myFunction()。
```

### Promise 对象：
```
"Producing code（生产代码）" 是需要一些时间的代码，
"Consuming code（消费代码）" 是必须等待结果的代码，
Promise 是一个 JavaScript 对象，它连接生成代码和消费代码。Promise 语法：
let myPromise = new Promise(function(myResolve, myReject) {
// "Producing Code"（可能需要一些时间）
  myResolve(); // 成功时
  myReject();  // 出错时
});
// "Consuming Code" （必须等待一个兑现的承诺）
myPromise.then(
  function(value) { /* 成功时的代码 */ },
  function(error) { /* 出错时的代码 */ }
);
当执行代码获得结果时，它应该调用两个回调之一：
结果	        调用
成功	        myResolve(result value)
出错	        myReject(error object)

Promise 对象属性
JavaScript Promise 对象可以是：Pending；Fulfilled；Rejected
Promise 对象支持两个属性：state 和 result。
当 Promise 对象 "pending"（工作）时，结果是 undefined。
当 Promise 对象 "fulfilled" 时，结果是一个值。
当一个 Promise 对象是 "rejected" 时，结果是一个错误对象。
myPromise.state	          myPromise.result
"pending"	                undefined
"fulfilled"	              结果值
"rejected"	              error 对象
您无法访问 Promise 属性 state 和 result。您必须使用 Promise 方法来处理 Promise。

如何使用 Promise
以下是使用 Promise 的方法：
myPromise.then(
  function(value) { /* code if successful */ },
  function(error) { /* code if some error */ }
);
Promise.then() 有两个参数，一个是成功时的回调，另一个是失败时的回调。两者都是可选的，因此您可以为成功或失败添加回调：
function myDisplayer(some) {
  document.getElementById("demo").innerHTML = some;
}
let myPromise = new Promise(function(myResolve, myReject) {
  let x = 0;
// 生成代码（这可能需要一些时间）
  if (x == 0) {
    myResolve("OK");
  } else {
    myReject("Error");
  }
});
myPromise.then(
  function(value) {myDisplayer(value);},
  function(error) {myDisplayer(error);}
);
```

### Async 和 await：
```
async 使函数返回 Promise，await 使函数等待 Promise。
Async 语法
函数前的关键字 async 使函数返回 promise：
async function myFunction() {
  return "Hello";
}
等同于：
async function myFunction() {
  return Promise.resolve("Hello");
}
以下是使用加上 Promise 的方法：
async function myFunction() {
  return "Hello";
}
myFunction().then(
  function(value) {myDisplayer(value);},
  function(error) {myDisplayer(error);}
);

Await 语法
函数前的关键字 await 使函数等待 promise：let value = await promise;await 关键字只能在 async 函数中使用。
等待超时
async function myDisplay() {
  let myPromise = new Promise(function(myResolve, myReject) {
    setTimeout(function() { myResolve("I love You !!"); }, 3000);
  });
  document.getElementById("demo").innerHTML = await myPromise;
}
myDisplay();
```

### HTML DOM：
```
通过 HTML DOM，JavaScript 能够访问和改变 HTML 文档的所有元素。当网页被加载时，浏览器会创建页面的文档对象模型（Document Object Model）。HTML DOM 模型被结构化为对象树。通过这个对象模型，JavaScript 获得创建动态 HTML 的所有力量：
JavaScript 能改变页面中的所有 HTML 元素
JavaScript 能改变页面中的所有 HTML 属性
JavaScript 能改变页面中的所有 CSS 样式
JavaScript 能删除已有的 HTML 元素和属性
JavaScript 能添加新的 HTML 元素和属性
JavaScript 能对页面中所有已有的 HTML 事件作出反应
JavaScript 能在页面中创建新的 HTML 事件

HTML DOM 是 HTML 的标准对象模型和编程接口。它定义了：
作为对象的 HTML 元素
所有 HTML 元素的属性
访问所有 HTML 元素的方法
所有 HTML 元素的事件
换言之：HTML DOM 是关于如何获取、更改、添加或删除 HTML 元素的标准。
```

### HTML DOM 方法：
```
HTML DOM 方法是您能够（在 HTML 元素上）执行的动作。HTML DOM 属性是您能够设置或改变的 HTML 元素的值。

DOM 编程界面
HTML DOM 能够通过 JavaScript 进行访问（也可以通过其他编程语言）。在 DOM 中，所有 HTML 元素都被定义为对象。编程界面是每个对象的属性和方法。属性是您能够获取或设置的值（就比如改变 HTML 元素的内容）。方法是您能够完成的动作（比如添加或删除 HTML 元素）。

下面的例子改变了 id="demo" 的 <p> 元素的内容：
<html>
<body>
<p id="demo"></p>
<script>
document.getElementById("demo").innerHTML = "Hello World!";
</script>
</body>
</html>
在上面的例子中，getElementById 是方法，而 innerHTML 是属性。

getElementById 方法
访问 HTML 元素最常用的方法是使用元素的 id。
在上面的例子中，getElementById 方法使用 id="demo" 来查找元素。
innerHTML 属性
获取元素内容最简单的方法是使用 innerHTML 属性。
innerHTML 属性可用于获取或替换 HTML 元素的内容。
innerHTML 属性可用于获取或改变任何 HTML 元素，包括 <html> 和 <body>。
```

### HTML DOM 文档：
```
HTML DOM 文档对象是您的网页中所有其他对象的拥有者。文档对象代表您的网页。如果您希望访问 HTML 页面中的任何元素，那么您总是从访问 document 对象开始。
查找 HTML 元素
方法	                                     描述
document.getElementById(id)	            通过元素 id 来查找元素
document.getElementsByTagName(name)	    通过标签名来查找元素
document.getElementsByClassName(name)	    通过类名来查找元素
改变 HTML 元素
方法	                                          描述
element.innerHTML = new html content	         改变元素的 inner HTML
element.attribute = new value	                 改变 HTML　元素的属性值
element.setAttribute(attribute, value)	         改变 HTML 元素的属性值
element.style.property = new style	         改变 HTML 元素的样式
添加和删除元素
方法	                                  描述
document.createElement(element)	        创建 HTML 元素
document.removeChild(element)	        删除 HTML 元素
document.appendChild(element)	        添加 HTML 元素
document.replaceChild(element)	        替换 HTML 元素
document.write(text)	                写入 HTML 输出流
添加事件处理程序
方法	                                                    描述
document.getElementById(id).onclick = function(){code}	向 onclick 事件添加事件处理程序
```

### HTML DOM 元素：
```
通常，通过 JavaScript，您需要操作 HTML 元素。为了达成此目的，您需要首先找到这些元素。有好几种完成此任务的方法：
通过 id 查找 HTML 元素
通过标签名查找 HTML 元素
通过类名查找 HTML 元素
通过 CSS 选择器查找 HTML 元素
通过 HTML 对象集合查找 HTML 元素

通过 id 查找 HTML 元素
DOM 中查找 HTML 元素最简单的方法是，使用元素的 id。本例查找 id="intro" 的元素：
var myElement = document.getElementById("intro");
(注：如果元素被找到，此方法会以对象返回该元素（在 myElement 中）。如果未找到元素，myElement 将包含 null。)
通过标签名查找 HTML 元素
本例查找所有 <p> 元素：
var x = document.getElementsByTagName("p");
通过类名查找 HTML 元素
如果您需要找到拥有相同类名的所有 HTML 元素，请使用 getElementsByClassName()。本例返回包含 class="intro" 的所有元素的列表：
var x = document.getElementsByClassName("intro");
通过 CSS 选择器查找 HTML 元素
如果您需要查找匹配指定 CSS 选择器（id、类名、类型、属性、属性值等等）的所有 HTML 元素，请使用 querySelectorAll() 方法。本例返回 class="intro" 的所有 <p> 元素列表：
var x = document.querySelectorAll("p.intro");
通过 HTML 对象选择器查找 HTML 对象
本例查找 id="frm1" 的 form 元素，在 forms 集合中，然后显示所有元素值：
var x = document.forms["frm1"];
var text = "";
 var i;
for (i = 0; i < x.length; i++) {
    text += x.elements[i].value + "<br>";
}
document.getElementById("demo").innerHTML = text;
```

### HTML DOM - 改变 HTML ：
```
HTML DOM 允许 JavaScript 改变 HTML 元素的内容。
改变 HTML 输出流
在 JavaScript 中，document.write() 可用于直接写入 HTML 输出流：
<script>
document.write(Date());
</script>
（注：千万不要在文档加载后使用 document.write()。这么做会覆盖文档。）

改变 HTML 内容
修改 HTML 文档内容最简单的方法是，使用 innerHTML 属性。如需修改 HTML 元素的内容，请使用此语法：
document.getElementById(id).innerHTML = new text
本例修改了 <p> 元素的内容：
<p id="p1">Hello World!</p>
<script>
document.getElementById("p1").innerHTML = "hello kitty!";
</script>

改变属性的值
如需修改 HTML 属性的值，请使用如下语法：
document.getElementById(id).attribute = new value
本例修改了 <img> 元素的 src 属性的值：
<img id="myImage" src="smiley.gif">
<script>
document.getElementById("myImage").src = "landscape.jpg";
</script>
```

### JavaScript 表单：
```
JavaScript 表单验证
HTML 表单验证可以通过 JavaScript 完成。如果表单域 (fname) 为空，该函数会提示一条消息，并返回 false，以防止表单被提交：
function validateForm() {
  let x = document.forms["myForm"]["fname"].value;
  if (x == "") {
    alert("Name must be filled out");
    return false;
  }
}

自动 HTML 表单验证
HTML 表单验证可以由浏览器自动执行：如果表单字段 (fname) 为空，则 required 属性会阻止提交此表单：
<form action="/action_page.php" method="post">
  <input type="text" name="fname" required>
  <input type="submit" value="Submit">
</form>

约束验证 HTML input 属性
属性	                    描述
disabled	           规定应禁用 input 元素。
max	                   规定 input 元素的最大值。
min	                   规定 input 元素的最小值。
pattern	                   规定 input 元素的值模式。
required	           规定 input 字段必填。
type	                   规定 input 元素的类型。
约束验证 CSS 伪选择器
选择器	                        描述
:disabled	              选择规定了 "disabled" 属性的 input 元素。
:invalid	              选择有无效值的 input 元素。
:optional	              选择未规定 "required" 属性的 input 元素。
:required	              选择规定了 "required" 属性的 input 元素。
:valid	                      选择具有有效值的 input 元素。
```

### HTML DOM - 改变 CSS :
```
HTML DOM 允许 JavaScript 更改 HTML 元素的样式。改变 HTML 样式,如需更改 HTML 元素的样式，请使用此语法：
document.getElementById(id).style.property = new style
下面的例子更改了 <p> 元素的样式：
<p id="p2">Hello World!</p>
<script>
document.getElementById("p2").style.color = "blue";
</script>
```

### HTML DOM 事件:
```
HTML 事件的例子：
当用户点击鼠标时
当网页加载后
当图像加载后
当鼠标移至元素上时
当输入字段被改变时
当 HTML 表单被提交时
当用户敲击按键时

HTML 事件属性
如需向 HTML 元素分配事件，您能够使用事件属性。向 button 元素分配 onclick 事件：
<button onclick="displayDate()">试一试</button>
在上例中，名为 displayDate 的函数会在按钮被点击时执行。

使用 HTML DOM 分配事件
HTML DOM 允许您使用 JavaScript 向 HTML 元素分配事件：为 button 元素指定 onclick 事件：
<script>
document.getElementById("myBtn").onclick = displayDate;
</script> 
在上例中，名为 displayDate 的函数被分配到 id="myBtn" 的 HTML 元素。当点击按钮时将执行函数。

onload 和 onunload 事件
当用户进入后及离开页面时，会触发 onload 和 onunload 事件。onload 事件可用于检测访问者的浏览器类型和浏览器版本，然后基于该信息加载网页的恰当版本。
onload 和 onunload 事件可用于处理 cookie:
<body onload="checkCookies()">

onchange 事件
onchange 事件经常与输入字段验证结合使用。下面是一个如何使用 onchange 的例子。当用户改变输入字段内容时，会调用 upperCase() 函数。
<input type="text" id="fname" onchange="upperCase()">

onmouseover 和 onmouseout 事件
onmouseover 和 onmouseout 事件可用于当用户将鼠标移至 HTML 元素上或移出时触发某个函数

onmousedown, onmouseup 以及 onclick 事件
onmousedown, onmouseup 以及 onclick 事件构成了完整的鼠标点击事件。首先当鼠标按钮被点击时，onmousedown 事件被触发；然后当鼠标按钮被释放时，onmouseup 事件被触发；最后，当鼠标点击完成后，onclick 事件被触发。
```

### HTML DOM 事件监听程序:
```
addEventListener() 方法为指定元素指定事件处理程序。addEventListener() 方法为元素附加事件处理程序而不会覆盖已有的事件处理程序。
您能够向一个元素添加多个事件处理程序。
您能够向一个元素添加多个相同类型的事件处理程序，例如两个 "click" 事件。
您能够向任何 DOM 对象添加事件处理程序而非仅仅 HTML 元素，例如 window 对象。
addEventListener() 方法使我们更容易控制事件如何对冒泡作出反应。
当使用 addEventListener() 方法时，JavaScript 与 HTML 标记是分隔的，已达到更佳的可读性；即使在不控制 HTML 标记时也允许您添加事件监听器。语法:
element.addEventListener(event, function, useCapture);
第一个参数是事件的类型（比如 "click" 或 "mousedown"）。
第二个参数是当事件发生时我们需要调用的函数。
第三个参数是布尔值，指定使用事件冒泡还是事件捕获。此参数是可选的。
(注：请勿对事件使用 "on" 前缀；请使用 "click" 代替 "onclick"。)

向元素添加事件处理程序
当用户点击某个元素时提示 "Hello World!"：
element.addEventListener("click", function(){ alert("Hello World!"); });
向相同元素添加多个事件处理程序
addEventListener() 方法允许您向相同元素添加多个事件，同时不覆盖已有事件：
element.addEventListener("click", myFunction);
element.addEventListener("click", mySecondFunction);
向 Window 对象添加事件处理程序
addEventListener() 允许您将事件监听器添加到任何 HTML DOM 对象上，比如 HTML 元素、HTML 对象、window 对象或其他支持事件的对象，比如 xmlHttpRequest 对象。添加当用户调整窗口大小时触发的事件监听器：
window.addEventListener("resize", function(){
    document.getElementById("demo").innerHTML = sometext;
});
传递参数
当传递参数值时，请以参数形式使用调用指定函数的“匿名函数”：
element.addEventListener("click", function(){ myFunction(p1, p2); });

在 HTML DOM 中有两种事件传播的方法：冒泡和捕获。
事件传播是一种定义当发生事件时元素次序的方法。假如 <div> 元素内有一个 <p>，然后用户点击了这个 <p> 元素，应该首先处理哪个元素“click”事件？
在冒泡中，最内侧元素的事件会首先被处理，然后是更外侧的：首先处理 <p> 元素的点击事件，然后是 <div> 元素的点击事件。
在捕获中，最外侧元素的事件会首先被处理，然后是更内侧的：首先处理 <div> 元素的点击事件，然后是 <p> 元素的点击事件。
在 addEventListener() 方法中，你能够通过使用“useCapture”参数来规定传播类型：
addEventListener(event, function, useCapture);
默认值是 false，将使用冒泡传播，如果该值设置为 true，则事件使用捕获传播。
document.getElementById("myP").addEventListener("click", myFunction, true);
document.getElementById("myDiv").addEventListener("click", myFunction, true);

removeEventListener() 方法
removeEventListener() 方法会删除已通过 addEventListener() 方法附加的事件处理程序：
element.removeEventListener("mousemove", myFunction);
```

### HTML DOM 导航:
```
DOM 节点
根据 W3C HTML DOM 标准，HTML 文档中的所有事物都是节点：
整个文档是文档节点
每个 HTML 元素是元素节点
HTML 元素内的文本是文本节点
每个 HTML 属性是属性节点
所有注释是注释节点在节点之间导航
通过 JavaScript，您可以使用以下节点属性在节点之间导航：
parentNode
childNodes[nodenumber]
firstChild
lastChild
nextSibling
previousSibling

DOM 根节点
有两个特殊属性允许访问完整文档：
document.body - 文档的 body
document.documentElement - 完整文档
<script>
 alert(document.body.innerHTML);
</script>

nodeName 属性
nodeName 属性规定节点的名称。nodeName 是只读的
元素节点的 nodeName 等同于标签名
属性节点的 nodeName 是属性名称
文本节点的 nodeName 总是 #text
文档节点的 nodeName 总是 #document
<h1 id="id01">我的第一张网页</h1>
<p id="id02">Hello!</p>
<script>
document.getElementById("id02").innerHTML  = document.getElementById("id01").nodeName;
</script>
(注：注释：nodeName 总是包含 HTML 元素的大写标签名。)

nodeValue 属性
nodeValue 属性规定节点的值。
元素节点的 nodeValue 是 undefined
文本节点的 nodeValue 是文本文本
属性节点的 nodeValue 是属性值

nodeType 属性
nodeType 属性返回节点的类型。nodeType 是只读的。
```

### HTML DOM 元素（节点）：
```
如需向 HTML DOM 添加新元素，您必须首先创建这个元素（元素节点），然后将其追加到已有元素。
<div id="div1">
<p id="p1">这是一个段落。</p>
<p id="p2">这是另一个段落。</p>
</div>
<script>
var para = document.createElement("p");                 // 这段代码创建了一个新的 <p> 元素
var node = document.createTextNode("这是新文本。");      // 如需向 <p> 元素添加文本，则必须首先创建文本节点。这段代码创建了一个文本节点
para.appendChild(node);                                 // 然后您需要向 <p> 元素追加这个文本节点
var element = document.getElementById("div1");          // 最后您需要向已有元素追加这个新元素。这段代码查找一个已有的元素
element.appendChild(para);                              // 这段代码向这个已有的元素追加新元素
</script>

创建新 HTML 元素 - insertBefore()
前面例子中的 appendChild() 方法，追加新元素作为父的最后一个子。
除此之外您还可以使用 insertBefore() 方法,追加新元素至旧元素之前：
element.insertBefore(para, child);

删除已有 HTML 元素
如需删除 HTML 元素，请使用 remove() 方法：
const elmnt = document.getElementById("p1"); 
elmnt.remove();

删除子节点
对于不支持 remove() 方法的浏览器，您必须找到父节点才能删除一个元素：
const parent = document.getElementById("div1");
const child = document.getElementById("p1");
parent.removeChild(child);

替换 HTML 元素
如需替换元素的，请使用 replaceChild() 方法：
parent.replaceChild(para, child);
```

### HTML DOM 集合：
```
HTMLCollection 对象
getElementsByTagName() 方法返回 HTMLCollection 对象。HTMLCollection 对象是类数组的 HTML 元素列表（集合）。下面的代码选取文档中的所有 <p> 元素：
var x = document.getElementsByTagName("p");
该集合中的元素可通过索引号进行访问。如需访问第二个 <p> 元素，您可以这样写：
y = x[1];
（注：索引从 0 开始。）

HTML HTMLCollection 长度
length 属性定义了 HTMLCollection 中元素的数量：
var myCollection = document.getElementsByTagName("p");
document.getElementById("demo").innerHTML = myCollection.length; 
```

### HTML DOM 节点列表：
```
NodeList 对象是从文档中提取的节点列表（集合）。NodeList 对象与 HTMLCollection 对象几乎相同。如使用 getElementsByClassName() 方法，某些（老的）浏览器会返回 NodeList 对象而不是 HTMLCollection。所有浏览器都会为 childNodes 属性返回 NodeList 对象。大多数浏览器会为 querySelectorAll() 方法返回 NodeList 对象。下面的代码选取文档中的所有 <p> 节点：
var myNodeList = document.querySelectorAll("p");

HTML DOM Node List 长度
length 属性定义节点列表中的节点数：
var myNodelist = document.querySelectorAll("p");
document.getElementById("demo").innerHTML = myNodelist.length;

HTMLCollection 与 NodeList 的区别
HTMLCollection（前一章）是 HTML 元素的集合。NodeList 是文档节点的集合。NodeList 和 HTML 集合几乎完全相同。HTMLCollection 和 NodeList 对象都是类数组的对象列表（集合）。它们都有定义列表（集合）中项目数的 length 属性。它们都可以通过索引 (0, 1, 2, 3, 4, ...) 像数组那样访问每个项目。访问 HTMLCollection 项目，可以通过它们的名称、id 或索引号。访问 NodeList 项目，只能通过它们的索引号。只有 NodeList 对象能包含属性节点和文本节点。节点列表不是数组！节点数组看起来像数组，但并不是。您能够遍历节点列表并像数组那样引用其节点。不过，您无法对节点列表使用数组方法，比如 valueOf()、push()、pop() 或 join()。
```

###　Window - 浏览器对象模型：
```
浏览器对象模型（Browser Object Model (BOM)）允许 JavaScript 与浏览器对话。

窗口尺寸
两个属性可用用于确定浏览器窗口的尺寸。这两个属性都以像素返回尺寸：
window.innerHeight - 浏览器窗口的内高度（以像素计）
window.innerWidth - 浏览器窗口的内宽度（以像素计）
浏览器窗口（浏览器视口）不包括工具栏和滚动条。
对于 Internet Explorer 8, 7, 6, 5：
document.documentElement.clientHeight
document.documentElement.clientWidth
或
document.body.clientHeight
document.body.clientWidth
该例显示浏览器窗口的高度和宽度：（不包括工具栏和滚动条）：
var w = window.innerWidth
|| document.documentElement.clientWidth
|| document.body.clientWidth;
var h = window.innerHeight
|| document.documentElement.clientHeight
|| document.body.clientHeight; 

其他窗口方法
一些其他方法：
window.open() - 打开新窗口
window.close() - 关闭当前窗口
window.moveTo() -移动当前窗口
window.resizeTo() -重新调整当前窗口
```

### Window Screen：
```
window.screen 对象包含用户屏幕的信息。window.screen 对象不带 window 前缀也可以写：
属性：
screen.width
screen.height
screen.availWidth
screen.availHeight
screen.colorDepth
screen.pixelDepth

Window Screen 宽度
screen.width 属性返回以像素计的访问者屏幕宽度。
document.getElementById("demo").innerHTML = "Screen Width: " + screen.width;
Window Screen 高度
screen.height 属性返回以像素计的访问者屏幕的高度。
document.getElementById("demo").innerHTML = "Screen Height: " + screen.height;
Window Screen 可用宽度
screen.availWidth 属性返回访问者屏幕的宽度，以像素计，减去诸如窗口工具条之类的界面特征。
document.getElementById("demo").innerHTML = "Available Screen Width: " + screen.availWidth;
Window Screen 可用高度
screen.availHeight 属性返回访问者屏幕的高度，以像素计，减去诸如窗口工具条之类的界面特征。
document.getElementById("demo").innerHTML = "Available Screen Height: " + screen.availHeight;

Window Screen 色深
screen.colorDepth 属性返回用于显示一种颜色的比特数。所有现代计算机都使用 24 位或 32 位硬件的色彩分辨率：
24 bits =16,777,216 种不同的 "True Colors"
32 bits = 4,294,967,296 中不同的 "Deep Colors"
更老的计算机使用 14 位：65,536 种不同的 "High Colors" 分辨率。异常古老的计算机，以及老式的手机使用 8 位：256 中不同的 "VGA colors"。
document.getElementById("demo").innerHTML = "Screen Color Depth: " + screen.colorDepth;
提示：HTML 中使用的 #rrggbb (rgb) 值代表 "True Colors" （16,777,216 中不同的颜色）。

Window Screen 像素深度
screen.pixelDepth 属性返回屏幕的像素深度。
document.getElementById("demo").innerHTML = "Screen Pixel Depth: " + screen.pixelDepth;
提示：对于现代计算机，颜色深度和像素深度是相等的。
```

### Window Location：
```
window.location 对象可用于获取当前页面地址（URL）并把浏览器重定向到新页面。window.location 对象可不带 window 前缀书写：
window.location.href 返回当前页面的 href (URL)
window.location.hostname 返回 web 主机的域名
window.location.pathname 返回当前页面的路径或文件名
window.location.protocol 返回使用的 web 协议（http: 或 https:）
window.location.assign 加载新文档

Window Location Href
window.location.href 属性返回当前页面的 URL。
document.getElementById("demo").innerHTML = "页面位置是 " + window.location.href;
Window Location 主机名
window.location.hostname 属性返回（当前页面的）因特网主机的名称。
document.getElementById("demo").innerHTML = "页面主机名是 " + window.location.hostname;
Window Location 路径名
window.location.pathname 属性返回当前页面的路径名。
document.getElementById("demo").innerHTML = "页面路径是 " + window.location.pathname;
Window Location 协议
window.location.protocol 属性返回页面的 web 协议。
document.getElementById("demo").innerHTML = "页面协议是 " + window.location.protocol;
Window Location 端口
window.location.port 属性返回（当前页面的）互联网主机端口的编号。
document.getElementById("demo").innerHTML = "端口号是： " + window.location.port;
提示：大多数浏览器不会显示默认端口号（http 为 80，https 为 443）。
Window Location Assign
window.location.assign() 方法加载新文档。
function newDoc() {
    window.location.assign("www.baidu.com")
 }
```

### Window History:
```
window.history 对象包含浏览器历史。window.history 对象可不带 window 书写。为了保护用户的隐私，JavaScript 访问此对象存在限制。
history.back() - 等同于在浏览器点击后退按钮
history.forward() - 等同于在浏览器中点击前进按钮

Window History Back
history.back() 方法加载历史列表中前一个 URL。这等同于在浏览器中点击后退按钮。
function goBack() {
    window.history.back()
 }

Window History Forward
history forward() 方法加载历史列表中下一个 URL。这等同于在浏览器中点击前进按钮。
function goForward() {
    window.history.forward()
 }
```

### Window Navigator:
```
window.navigator 对象包含有关访问者的信息。

浏览器 Cookie，cookieEnabled 属性返回 true，如果 cookie 已启用，否则返回 false。
浏览器应用程序名称，appName 属性返回浏览器的应用程序名称。提示："Netscape" 是 IE11、Chrome、Firefox 以及 Safari 的应用程序名称的统称。
浏览器应用程序代码名称，appCodeName 属性返回浏览器的应用程序代码名称。提示："Mozilla" 是 Chrome、Firefox、IE、Safari 以及 Opera 的应用程序代码名称。
浏览器引擎，product 属性返回浏览器引擎的产品名称。
浏览器版本，appVersion 属性返回有关浏览器的版本信息。
浏览器代理，userAgent 属性返回由浏览器发送到服务器的用户代理报头（user-agent header）。
浏览器平台，platform 属性返回浏览器平台（操作系统）。
浏览器语言，language 属性返回浏览器语言。
浏览器是否在线?onLine 属性返回 true，假如浏览器在线。
Java 是否启用?javaEnabled() 方法返回 true，如果 Java 已启用。
(注：来自 navigator 对象的信息通常是误导性的，不应该用于检测浏览器版本，因为：
不同浏览器能够使用相同名称
导航数据可被浏览器拥有者更改
某些浏览器会错误标识自身以绕过站点测试
浏览器无法报告发布晚于浏览器的新操作系统)
```

### 弹出框：
```
JavaScript 有三种类型的弹出框：警告框、确认框和提示框。

警告框
如果要确保信息传递给用户，通常会使用警告框。当警告框弹出时，用户将需要单击“确定”来继续。语法：
window.alert("sometext");
window.alert() 方法可以不带 window 前缀来写。

确认框
如果您希望用户验证或接受某个东西，则通常使用“确认”框。当确认框弹出时，用户将不得不单击“确定”或“取消”来继续进行。如果用户单击“确定”，该框返回 true。如果用户单击“取消”，该框返回 false。语法：
window.confirm("sometext");
window.confirm() 方法可以不带 window 前缀来编写。

提示框
如果您希望用户在进入页面前输入值，通常会使用提示框。当提示框弹出时，用户将不得不输入值后单击“确定”或点击“取消”来继续进行。如果用户单击“确定”，该框返回输入值。如果用户单击“取消”，该框返回 NULL。语法：
window.prompt("sometext","defaultText");
window.prompt() 方法可以不带 window 前缀来编写。

折行
如需在弹出框中显示折行，请在反斜杠后面加一个字符 n。
alert("Hello\nHow are you?");
```

### Timing 事件：
```
Timing 事件
window 对象允许以指定的时间间隔执行代码。这些时间间隔称为定时事件。通过 JavaScript 使用的有两个关键的方法：
setTimeout(function, milliseconds)
在等待指定的毫秒数后执行函数。
setInterval(function, milliseconds)
等同于 setTimeout()，但持续重复执行该函数。
setTimeout() 和 setInterval() 都属于 HTML DOM Window 对象的方法。

setTimeout() 方法
window.setTimeout(function, milliseconds);
window.setTimeout() 方法可以不带 window 前缀来编写。第一个参数是要执行的函数。第二个参数指示执行之前的毫秒数。
如何停止执行？
clearTimeout() 方法停止执行 setTimeout() 中规定的函数。
window.clearTimeout(timeoutVariable)
window.clearTimeout() 方法可以不带 window 前缀来写。clearTimeout() 使用从 setTimeout() 返回的变量：
myVar = setTimeout(function, milliseconds);
clearTimeout(myVar);

setInterval() 方法
setInterval() 方法在每个给定的时间间隔重复给定的函数。
window.setInterval(function, milliseconds);
window.setInterval() 方法可以不带 window 前缀来写。第一个参数是要执行的函数。第二个参数每个执行之间的时间间隔的长度。
如何停止执行？
clearInterval() 方法停止 setInterval() 方法中指定的函数的执行。
window.clearInterval(timerVariable)
window.clearInterval() 方法可以不带 window 前缀来写。clearInterval() 方法使用从 setInterval() 返回的变量：
myVar = setInterval(function, milliseconds);
clearInterval(myVar);
```

### Cookies：
```
什么是 cookie？
Cookie 是在您的计算机上存储在小的文本文件中的数据。当 web 服务器向浏览器发送网页后，连接被关闭，服务器会忘记用户的一切。Cookie 是为了解决“如何记住用户信息”而发明的：
当用户访问网页时，他的名字可以存储在 cookie 中。
下次用户访问该页面时，cookie 会“记住”他的名字。
Cookie 保存在名称值对中，如：
username = Bill Gates
当浏览器从服务器请求一个网页时，将属于该页的 cookie 添加到该请求中。这样服务器就获得了必要的数据来“记住”用户的信息。如果浏览器已关闭本地 cookie 支持，则以下实例均无法工作。

通过 JavaScript 创建 cookie
JavaScript 可以用 document.cookie 属性创建、读取、删除 cookie。
通过 JavaScript，可以这样创建 cookie：
document.cookie = "username=Bill Gates";
您还可以添加有效日期（UTC 时间）。默认情况下，在浏览器关闭时会删除 cookie：
document.cookie = "username=Bill Gates; expires=Sun, 31 Dec 2017 12:00:00 UTC";
通过 path 参数，您可以告诉浏览器 cookie 属于什么路径。默认情况下，cookie 属于当前页。
document.cookie = "username=Bill Gates; expires=Sun, 31 Dec 2017 12:00:00 UTC; path=/";

通过 JavaScript 读取 cookie
通过 JavaScript，可以这样读取 cookie：
var x = document.cookie;
document.cookie 会在一条字符串中返回所有 cookie，比如：cookie1=value; cookie2=value; cookie3=value;

通过 JavaScript 改变 cookie
通过使用 JavaScript，你可以像你创建 cookie 一样改变它：
document.cookie = "username=Steve Jobs; expires=Sun, 31 Dec 2017 12:00:00 UTC; path=/";
旧 cookie 被覆盖。

通过 JavaScript 删除 cookie
删除 cookie 非常简单。删除 cookie 时不必指定 cookie 值：直接把 expires 参数设置为过去的日期即可：
document.cookie = "username=; expires=Thu, 01 Jan 1970 00:00:00 UTC; path=/;";
您应该定义 cookie 路径以确保删除正确的 cookie。如果你不指定路径，一些浏览器不会让你删除 cookie。

JavaScript Cookie 实例
在下面的示例中，我们将创建一个 cookie 来存储访问者的名称。访客第一次到达网页时，会要求他填写姓名。然后将该名称存储在 cookie 中。下次访客到达同一页时，他将收到一条欢迎消息。例如，我们将创建 3 个JavaScript函数：
设置 cookie 值的函数
获取 cookie 值的函数
检查 cookie 值的函数
function setCookie(cname, cvalue, exdays) {                    // 设置 cookie 值的函数
    var d = new Date();
    d.setTime(d.getTime() + (exdays * 24 * 60 * 60 * 1000));
    var expires = "expires="+d.toUTCString();
    document.cookie = cname + "=" + cvalue + ";" + expires + ";path=/";
}
function getCookie(cname) {                                    // 获取 cookie 值的函数
    var name = cname + "=";
    var ca = document.cookie.split(';');
    for(var i = 0; i < ca.length; i++) {
        var c = ca[i];
        while (c.charAt(0) == ' ') {
            c = c.substring(1);
         }
        if (c.indexOf(name)  == 0) {
            return c.substring(name.length, c.length);
         }
    }
    return "";
}
function checkCookie() {                                       // 检查 cookie 值的函数
    var user = getCookie("username");
    if (user != "") {
        alert("Welcome again " + user);
    } else {
        user = prompt("Please enter your name:", "");
        if (user != "" && user != null) {
            setCookie("username", user, 365);
        }
    }
}
```

### Web API - 简介:
```
Web API 是开发人员的梦想。它可以扩展浏览器的功能;它可以极大简化复杂的功能;它可以为复杂的代码提供简单的语法。
API 指的是应用程序编程接口（Application Programming Interface）。
Web API 是 Web 的应用程序编程接口。
浏览器 API 可以扩展 Web 浏览器的功能。
服务器 API 可以扩展 Web 服务器的功能。
```

### 验证 API：
```
约束验证 DOM 方法
属性	                  描述
checkValidity()	         如果 input 元素包含有效数据，则返回 true。
setCustomValidity()	 设置 input 元素的 validationMessage 属性。

约束验证 DOM 属性
属性	                  描述
validity	          包含与输入元素有效性相关的布尔属性。
validationMessage	  包含当有效性为 false 时浏览器将显示的消息。
willValidate	          指示是否将验证 input 元素。

validity属性
input 元素的 validity 属性包含一系列关于 validity 数据属性：
属性	                   描述
customError	          如果设置了自定义有效性消息，则设置为 true。
patternMismatch	          如果元素的值与其 pattern 属性不匹配，则设置为 true。
rangeOverflow	          如果元素的值大于其 max 属性，则设置为 true。
rangeUnderflow	          如果元素的值小于其 min 属性，则设置为 true。
stepMismatch	          如果元素的值对其 step 属性无效，则设置为 true。
tooLong	                  如果元素的值超过其 maxLength 属性，则设置为 true。
typeMismatch	          如果元素的值对其 type 属性无效，则设置为 true。
valueMissing	          如果元素（具有 required 属性）没有值，则设置为 true。
valid	                  如果元素的值有效，则设置为 true。
```

### History API：
```
Web History API 提供了访问 windows.history 对象的简单方法。window.history 对象包含用户访问过的 URL（网站）。
History 对象属性
属性	            描述
length	         返回历史列表中的 URL 数量。
History          对象方法
方法	          描述
back()	          加载历史列表中的上一个 URL。
forward()	  加载历史列表中的下一个 URL。
go()	          从历史列表中加载特定的 URL。
```

### Web Storage API：
```
Web Storage API 是一种用于在浏览器中存储和检索数据的简单语法。他非常容易使用。
localStorage 对象
localStorage 对象提供对特定网站的本地存储的访问。它允许您存储、读取、添加、修改和删除该域的数据项。存储的数据没有到期日期，并且在浏览器关闭时不会被删除。这些数据将在几天、几周和几年内均可用。
setItem() 方法
localStorage.setItem() 方法将数据项存储在 storage 中。它接受一个名称和一个值作为参数：
localStorage.setItem("name", "Bill Gates");
getItem() 方法
localStorage.getItem() 方法从存储（storage）中检索数据项。它接受一个名称作为参数：
localStorage.getItem("name");

sessionStorage 对象
sessionStorage 对象与 localStorage 对象相同。不同之处在于 sessionStorage 对象存储会话的数据。当浏览器关闭时，数据会被删除。
setItem() 方法
sessionStorage.setItem() 方法将数据项存储在存储（storage）中。它接受一个名称和一个值作为参数：
sessionStorage.setItem("name", "Bill Gates");
getItem() 方法
sessionStorage.getItem() 方法从存储（storage）中检索数据项。它接受一个名称作为参数：
sessionStorage.getItem("name");

Storage 对象属性和方法
属性/方法	                       描述
key(n)	                          返回存储中第 n 个键的名称。
length	                          返回存储在 Storage 对象中的数据项数。
getItem(keyname)	          返回指定的键名的值。
setItem(keyname, value)	          将键添加到存储中，或者如果键已经存在，则更新该键的值。
removeItem(keyname)	          从存储中删除该键。
clear()	                          清空所有键。
Web Storage API 相关页面
属性	                        描述
window.localStorage	        允许在 Web 浏览器中保存键/值对。存储没有到期日期的数据。
window.sessionStorage	        允许在 Web 浏览器中保存键/值对。存储一个会话的数据。
```

### Web Worker API：
```
Web Worker 是在后台运行的 JavaScript，独立于其他脚本，不会影响页面的性能。你可以继续做任何你想做的事情：点击、选取内容等，同时 web worker 在后台运行。

创建 Web Worker 对象
假设我们有了 web worker 文件，我们需要从 HTML 页面调用它。以下代码行检查 worker 是否已存在，如果不存在，它会创建一个新的 web worker 对象并运行 "demo_workers.js" 中的代码：
if (typeof(w) == "undefined") {
  w = new Worker("demo_workers.js");
}
终止 Web Worker
当 web worker 对象被创建时，它会继续监听消息（即使在外部脚本完成之后）直到它被终止。如需终止 web worker，并释放浏览器/计算机资源，请使用 terminate() 方法：
w.terminate();
重用 Web Worker
如果将 worker 变量设置为 undefined，则在它终止后，您可以重用以下代码：
w = undefined;

Web Worker 和 DOM
由于 Web Worker 位于外部文件中，因此他们无法访问以下 JavaScript 对象：
window 对象
document 对象
parent 对象

Fetch API：
Fetch API 接口允许 Web 浏览器向 Web 服务器发出 HTTP 请求。不再需要 XMLHttpRequest。
下面的例子获取文件并显示内容，由于 Fetch 基于 async 和 await：
async function getText(file) {
  let x = await fetch(file);
  let y = await x.text();
  myDisplay(y);
}
```

### Web Geolocation API：
```
HTML Geolocation API 用于获取用户的地理位置。由于这可能会损害隐私，除非用户批准，否则位置不可用。（注：地理定位对于带有 GPS 的设备（如智能手机）最为准确。）

使用 Geolocation API
getCurrentPosition() 方法用于返回用户的位置。getCurrentPosition() 方法在成功时返回一个对象。会始终返回纬度、经度和精度属性。如果可用，则返回其他属性：
属性	                         返回
coords.latitude	              以十进制数表示的纬度（始终返回）。
coords.longitude	      以十进制数表示的经度（始终返回）。
coords.accuracy	              位置精度（始终返回）。
coords.altitude	              平均海平面以上的高度（以米计）（如果可用则返回）。
coords.altitudeAccuracy	      位置的高度精度（如果可用则返回）。
coords.heading	              从北顺时针方向的航向（如果可用则返回）。
coords.speed	              以米/秒计的速度（如果可用则返回）。
timestamp	              响应的日期/时间（如果可用则返回）。

Geolocation 对象还有其他有趣的方法：
watchPosition() - 返回用户的当前位置，并随着用户移动（如汽车中的 GPS）继续返回更新的位置。
clearWatch() - 停止 watchPosition () 方法。
```

### AJAX 简介：
```
AJAX 是开发者的梦想，因为您能够：
不刷新页面更新网页
在页面加载后从服务器请求数据
在页面加载后从服务器接收数据
在后台向服务器发送数据

什么是 AJAX？
AJAX = Asynchronous JavaScript And XML.AJAX 并非编程语言。AJAX 仅仅组合了：
浏览器内建的 XMLHttpRequest 对象（从 web 服务器请求数据）
JavaScript 和 HTML DOM（显示或使用数据）
Ajax 是一个令人误导的名称。Ajax 应用程序可能使用 XML 来传输数据，但将数据作为纯文本或 JSON 文本传输也同样常见。
Ajax 允许通过与场景后面的 Web 服务器交换数据来异步更新网页。这意味着可以更新网页的部分，而不需要重新加载整个页面。

AJAX 如何工作
1.网页中发生一个事件（页面加载、按钮点击）
2.由 JavaScript 创建 XMLHttpRequest 对象
3.XMLHttpRequest 对象向 web 服务器发送请求
4.服务器处理该请求
5.服务器将响应发送回网页
6.由 JavaScript 读取响应
7.由 JavaScript 执行正确的动作（比如更新页面）
```

### AJAX - XMLHttpRequest：
```
创建 XMLHttpRequest 对象
所有现代浏览器（Chrom、IE7+、Firefox、Safari 以及 Opera）都有内建的 XMLHttpRequest 对象。
创建 XMLHttpRequest 的语法是：variable = new XMLHttpRequest();
老版本的 Internet Explorer（IE5 和 IE6）使用 ActiveX 对象：variable = new ActiveXObject("Microsoft.XMLHTTP");

XMLHttpRequest 对象用于同服务器交换数据。
方法	                          描述
open(method, url, async)	规定请求的类型
                                method：请求的类型：GET 还是 POST
                                url：服务器（文件）位置
                                async：true（异步）或 false（同步）
send()	                        向服务器发送请求（用于 GET）
send(string)	                向服务器发送请求（用于 POST）

GET 比 POST 更简单更快，可用于大多数情况下。不过，请在以下情况始终使用 POST：
缓存文件不是选项（更新服务器上的文件或数据库）
向服务器发送大量数据（POST 无大小限制）
发送用户输入（可包含未知字符），POST 比 GET 更强大更安全

一条简单的 GET 请求：
xhttp.open("GET", "demo_get.asp", true);
xhttp.send();
在上面的例子中，您可能会获得一个缓存的结果。为了避免此情况，请向 URL 添加一个唯一的 ID：
xhttp.open("GET", "demo_get.asp?t=" + Math.random(), true);
xhttp.send();
如果您需要用 GET 方法来发送信息，请向 URL 添加这些信息：
xhttp.open("GET", "demo_get2.asp?fname=Bill&lname=Gates", true);
xhttp.send();

一条简单的 POST 请求：
xhttp.open("POST", "demo_post.asp", true);
xhttp.send();
如需像 HTML 表单那样 POST 数据，请通过 setRequestHeader() 添加一个 HTTP 头部。请在 send() 方法中规定您需要发送的数据：
xhttp.open("POST", "ajax_test.asp", true);
xhttp.setRequestHeader("Content-type", "application/x-www-form-urlencoded");
xhttp.send("fname=Bill&lname=Gates");
方法	                                      描述
setRequestHeader(header, value)	           向请求添加 HTTP 头部
                                           header：规定头部名称
                                           value：规定头部值

AJAX - 服务器响应：
属性	                            描述
onreadystatechange	     定义了当 readyState 属性发生改变时所调用的函数。
readyState	             保存了 XMLHttpRequest 的状态。
                             0: 请求未初始化
                             1: 服务器连接已建立
                             2: 请求已接收
                             3: 正在处理请求
                             4: 请求已完成且响应已就绪
status	                     200: "OK"
                             403: "Forbidden"
                             404: "Page not found"
statusText	                 返回状态文本（例如 "OK" 或 "Not Found"）
提示：每当 readyState 发生变化时就会调用 onreadystatechange 函数。
当 readyState 为 4，status 为 200 时，响应就绪：
function loadDoc() {
    var xhttp = new XMLHttpRequest();
    xhttp.onreadystatechange = function() {
        if (this.readyState == 4 && this.status == 200) {
            document.getElementById("demo").innerHTML =
            this.responseText;
       }
    };
    xhttp.open("GET", "ajax_info.txt", true);
    xhttp.send(); 
} 
（注：onreadystatechange 被触发五次（0-4），每次 readyState 都发生变化。）

使用回调函数
回调函数是一种作为参数被传递到另一个函数的函数。如果您的网站中有多个 AJAX 任务，那么您应该创建一个执行 XMLHttpRequest 对象的函数，以及一个供每个 AJAX 任务的回调函数。该函数应当包含 URL 以及当响应就绪时调用的函数。
loadDoc("url-1", myFunction1);
function loadDoc(url, cFunction) {
  var xhttp;
  xhttp = new XMLHttpRequest();
  xhttp.onreadystatechange = function() {
    if (this.readyState == 4 && this.status == 200) {
      cFunction(this);
    }
  };
  xhttp.open("GET", url, true);
  xhttp.send();
}
function myFunction1(xhttp) {
  // 行动在这里
 } 

服务器响应属性
属性	                  描述
responseText	        获取字符串形式的响应数据
responseXML	        获取 XML 数据形式的响应数据
服务器响应方法
方法	                         描述
getResponseHeader()	      从服务器返回特定的头部信息
getAllResponseHeaders()	      从服务器返回所有头部信息

responseText 属性以 JavaScript 字符串的形式返回服务器响应，因此您可以这样使用它：
document.getElementById("demo").innerHTML = xhttp.responseText;
XML HttpRequest 对象有一个內建的 XML 解析器。ResponseXML 属性以 XML DOM 对象返回服务器响应。使用此属性，您可以把响应解析为 XML DOM 对象：
xmlDoc = xhttp.responseXML;
txt = "";
x = xmlDoc.getElementsByTagName("ARTIST");
for (i = 0; i < x.length; i++) {
  txt += x[i].childNodes[0].nodeValue + "<br>";
  }
document.getElementById("demo").innerHTML = txt;
xhttp.open("GET",  "music_list.xml", true);
xhttp.send();
getAllResponseHeaders() 方法返回所有来自服务器响应的头部信息。
var xhttp = new XMLHttpRequest();
xhttp.onreadystatechange = function() {
  if (this.readyState == 4 && this.status == 200) {
    document.getElementById("demo").innerHTML = this.getAllResponseHeaders();
  }
};
getResponseHeader() 方法返回来自服务器响应的特定头部信息。
var xhttp = new XMLHttpRequest();
xhttp.onreadystatechange = function() {
  if (this.readyState == 4 && this.status == 200) {
    document.getElementById("demo").innerHTML = this.getResponseHeader("Last-Modified");
  }
};
xhttp.open("GET", "ajax_info.txt", true);
xhttp.send(); 
```

### JSON 简介：
```
JSON: JavaScript Object Notation（JavaScript 对象标记法）。JSON 是一种存储和交换数据的语法。JSON 是通过 JavaScript 对象标记法书写的文本。
什么是 JSON？
JSON 指的是 JavaScript 对象标记法（JavaScript Object Notation）
JSON 是一种轻量级的数据交换格式
JSON 具有自我描述性且易于理解
JSON 独立于语言*
JSON 使用 JavaScript 语法，但是 JSON 格式是纯文本的。文本可被任何编程语言作为数据来读取和使用。JSON 格式最初由 Douglas Crockford 提出。

为什么使用 JSON？
因为 JSON 格式仅仅是文本，它能够轻松地在服务器浏览器之间传输，并用作任何编程语言的数据格式。
JavaScript 提供內建函数把以 JSON 格式写的字符串转换为原生 JavaScript 对象：
JSON.parse()
因此，如果您以 JSON 格式从服务器接收数据，那么您可以像任何其他 JavaScript 对象那样使用它。
```

### JSON 语法：
```
JSON 语法规则，JSON 语法衍生于 JavaScript 对象标记法语法：
数据在名称/值对中
数据由逗号分隔
花括号容纳对象
方括号容纳数组

JSON 数据写为名称/值对。名称/值由字段名称构成，后跟冒号和值：
"name":"Bill Gates"
JSON 名称需要双引号。而 JavaScript 名称不需要。JSON – 求值为 JavaScript 对象JSON 格式几乎等同于 JavaScript 对象。
在 JSON 中，键必须是字符串，由双引号包围：
JSON
{ "name":"Bill Gates" }
在 JavaScript 中，键可以是字符串、数字或标识符名称：
JavaScript
{ name:"Bill Gates" }

在 JSON 中，值必须是以下数据类型之一：
字符串；数字；对象（JSON 对象）；数组；布尔；null
在 JavaScript 中，以上所列均可为值，外加其他有效的 JavaScript 表达式，包括：
函数；日期；undefined
在 JSON 中，字符串值必须由双引号编写：
JSON
{ "name":"Bill Gates" }
在 JavaScript 中，您可以书写使用双引号或单引号的字符串值：
JavaScript
{ name:'Bill Gates' }

因为 JSON 语法由 JavaScript 对象标记法衍生而来，所以很少需要其他额外的软件来处理 JavaScript 中的 JSON。通过 JavaScript，您能够创建对象并向其分配数据，就像这样：
var person =  { name : "Bill Gates", age : 62, city : "Seattle" };
您能够像这样访问 JavaScript 对象：
// 返回 Bill Gates
person.name;
也可以像这样访问它：
// 返回 Bill Gates
person["name"];
可以像这样修改数据：
person.name = "Steve Jobs";
也可以像这样修改它：
person["name"] = "Steve Jobs";

JSON 文件
JSON 文件的文件类型是 ".json"
JSON 文本的 MIME 类型是 "application/json"
```

### JSON vs XML：
```
JSON 和 XML 均可用于从 web 服务器接收数据。下面的 JSON 和 XML 实例都定义了雇员对象，包含了由 3 个雇员构成的数组：
JSON 实例
{"employees":[
    { "firstName":"Bill", "lastName":"Gates" },
    { "firstName":"Steve", "lastName":"Jobs" },
    { "firstName":"Elon", "lastName":"Musk" }
]}
XML 实例
<employees>
    <employee>
         <firstName>Bill</firstName>
         <lastName>Gates</lastName>
     </employee>
     <employee>
         <firstName>Steve</firstName>
         <lastName>Jobs</lastName>
     </employee>
     <employee>
         <firstName>Elon</firstName>
         <lastName>Musk</lastName>
     </employee>
</employees>

JSON 类似 XML，因为:
JSON 和 XML 都是“自描述的”（人类可读的）
JSON 和 XML 都是分级的（值中有值）
JSON 和 XML 都能被大量编程语言解析和使用
JSON 和 XML 都能被 XMLHttpRequest 读取

JSON 与 XML 的差异在于：
JSON 不使用标签
JSON 更短
JSON 的读写速度更快
JSON 可使用数组
最大的不同在于：
XML 必须使用 XML 解析器进行解析。而 JSON 可通过标准的 JavaScript 函数进行解析。

为什么 JSON 比 XML 更好？
XML 比 JSON 更难解析。
JSON 被解析为可供使用的 JavaScript 对象。
对于 AJAX 应用程序，JSON 比 XML 更快更易用：
使用 XML：
读取 XML 文档
使用 XML DOM 遍历文档
提取变量中存储的值
使用 JSON：
读取 JSON 字符串
JSON.Parse JSON 字符串
```

### JSON 数据类型：
```
有效的数据类型
在 JSON 中，值必须是以下数据类型之一：
字符串；数字；对象（JSON 对象）；数组；布尔；Null
JSON 的值不可以是以下数据类型之一：
函数；日期；undefined

JSON 中的字符串必须用双引号包围。
{ "name":"Bill" }
JSON 中的数字必须是整数或浮点数。
{ "age":30 }
JSON 中的值可以是对象。
{"employee":{ "name":"Bill Gates", "age":62, "city":"Seattle" }}（注：JSON 中作为值的对象必须遵守与 JSON 对象相同的规则。）
JSON 中的值可以是数组。
{"employees":[ "Bill", "Steve", "David" ]}
JSON 中的值可以是 true/false。
{ "sale":true }
JSON 中的值可以是 null。
{ "middlename":null }
```

### JSON.parse()：
```
JSON 的常规用途是同 web 服务器进行数据传输。在从 web 服务器接收数据时，数据永远是字符串。通过 JSON.parse() 解析数据，这些数据会成为 JavaScript 对象。

解析 JSON
请想象一下我们从 web 服务器接收到这段文本：
'{ "name":"Bill Gates", "age":62, "city":"Seattle"}'
请使用 JavaScript 函数 JSON.parse() 把文本转换为 JavaScript 对象：
var obj = JSON.parse('{ "name":"Bill Gates", "age":62, "city":"Seattle"}');
（注：请确保这段文本以 JSON 格式书写，否则会出现语法错误。）

来自服务器的 JSON
您能够通过使用 AJAX 请求从服务器请求 JSON。只要服务器的响应是用 JSON 格式编写的，你可以将字符串解析成 JavaScript 对象。请使用 XMLHttpRequest 从服务器获取数据：
var xmlhttp = new XMLHttpRequest();
xmlhttp.onreadystatechange = function()  {
    if (this.readyState == 4 && this.status == 200) {
        myObj =  JSON.parse(this.responseText);
        document.getElementById("demo").innerHTML  = myObj.name;
    }
};
xmlhttp.open("GET", "json_demo.txt", true);
xmlhttp.send();

作为 JSON 的数组
在对衍生自数组的 JSON 使用 JSON.parse() 后，此方法将返回 JavaScript 数组，而不是 JavaScript 对象。从服务器返回的 JSON 是数组：
var xmlhttp = new XMLHttpRequest();
xmlhttp.onreadystatechange = function()  {
    if (this.readyState == 4 && this.status == 200) {
        myArr =  JSON.parse(this.responseText);
        document.getElementById("demo").innerHTML  = myArr[0];
    }
};
xmlhttp.open("GET", "json_demo_array.txt", true);
xmlhttp.send();

解析日期
JSON 中不允许日期对象。如果您需要包含日期，请写为字符串。之后您可以将其转换回日期对象：把字符串转换为日期：
var text =  '{ "name":"Bill Gates", "birth":"1955-10-28", "city":"Seattle"}';
var obj = JSON.parse(text);
obj.birth = new Date(obj.birth);
document.getElementById("demo").innerHTML = obj.name + ", " + obj.birth;
或者您可以已使用 JSON.parse() 函数的第二个参数，被称为 reviver。这个 reviver 参数是函数，在返回值之前，它会检查每个属性。将字符串转换为日期，使用 reviver 函数：
var text =  '{ "name":"Bill Gates", "birth":"1955-10-28", "city":"Seattle"}';
var obj = JSON.parse(text, function (key, value) {
    if  (key == "birth") {
        return new Date(value);
    } else {
         return value;
   }});
document.getElementById("demo").innerHTML = obj.name + ", " + obj.birth;

解析函数
JSON 中不允许函数。如果您需要包含函数，请把它写作字符串。稍后您可以把它转换回函数：把字符串转换为函数：
var text =  '{ "name":"Bill Gates", "age":"function () {return 62;}", "city":"Seattle"}';
var obj = JSON.parse(text);
obj.age = eval("(" + obj.age + ")");
document.getElementById("demo").innerHTML = obj.name + ", " +  obj.age();
（注：您应该避免在 JSON 中使用函数，函数会丢失它们的作用域，而且您还需要使用 eval() 把它们转换回函数。）
```

### JSON.stringify()：
```
JSON 的常规用途是同 web 服务器进行数据交换。在向 web 服务器发送数据时，数据必须是字符串。通过 JSON.stringify() 把 JavaScript 对象转换为字符串。

对 JavaScript 对象进行字符串化
想象一下我们在 JavaScript 中有这个对象：
var obj = { name:"Bill Gates", age:62, city:"Seattle"};
请使用 JavaScript 函数 JSON.stringify() 将它转换为字符串。
var myJSON = JSON.stringify(obj);
结果将是遵守 JSON 标记法的一段字符串。

Stringify JavaScript 数组
也可以对 JavaScript 数组进行字符串化：想象一下我们在 JavaScript中有这个数组：
var arr = [ "Bill Gates", "Steve Jobs", "Elon Musk" ];
请使用 JavaScript 函数 JSON.stringify() 将其转换为字符串。
var myJSON = JSON.stringify(arr);
结果将是遵守 JSON 标记法的字符串。

日期字符串化
在 JSON 中，不允许日期对象。JSON.stringify() 函数将把任何日期转换为字符串。
var obj =  { "name":"Bill Gates", "today":new Date(), "city":"Seattle"};
var myJSON = JSON.stringify(obj);
document.getElementById("demo").innerHTML = myJSON;
您可以在接收端把字符串转换回日期对象。

函数字符串化
在 JSON 中，不允许函数作为对象值。JSON.stringify() 函数将从 JavaScript 对象删除任何函数，包括键和值：
var obj =  { "name":"Bill Gates", "age":function () {return 62;}, "city":"Seattle"};
var myJSON = JSON.stringify(obj);
document.getElementById("demo").innerHTML = myJSON;   // myJSON 返回 {"name":"Bill Gates","city":"Seattle"}
如果您在运行 JSON.stringify() 函数前已将函数转换为字符串，这个环节可以省略。
var obj =  { "name":"Bill Gates", "age":function () {return 62;}, "city":"Seattle"};
obj.age = obj.age.toString();
var myJSON = JSON.stringify(obj);
document.getElementById("demo").innerHTML = myJSON;   // myJSON 返回 {"name":"Bill Gates","age":"function () {return 62;}","city":"Seattle"}
（注：您应该避免在 JSON 中使用函数，函数会失去其作用域，而且您还需要使用 eval() 将它们转换回函数。）
```

### JSON 对象：
```
对象语法
{ "name":"Bill Gates", "age":62, "car":null }
JSON 对象被花括号 {} 包围。JSON 对象以键/值对书写。键必须是字符串，值必须是有效的 JSON 数据类型（字符串、数字、对象、数组、布尔或 null）。键和值由冒号分隔。每个键/值对由逗号分隔。

访问对象值
您可以通过使用点号（.）来访问对象值：
myObj =  { "name":"Bill Gates", "age":62, "car":null };
x = myObj.name;
您也可以使用方括号（[]）来访问对象值：
myObj =  { "name":"Bill Gates", "age":62, "car":null };
x = myObj["name"];

遍历对象
您能够通过使用 for-in 遍历对象属性：
myObj =  { "name":"Bill Gates", "age":62, "car":null };
for (x in myObj) {
   document.getElementById("demo").innerHTML  += x;
}
在 for-in 循环中，请使用括号标记法来访问属性值：
myObj =  { "name":"Bill Gates", "age":62, "car":null };
for (x in myObj) {
   document.getElementById("demo").innerHTML  += myObj[x];
}

嵌套的 JSON 对象
一个 JSON 对象中的值可以是另一个 JSON 对象。
myObj =  {
   "name":"Bill Gates",
   "age":62,
   "cars": {
	  "car1":"Porsche",
	  "car2":"BMW",
	  "car3":"Volvo"
   }
}
您能够通过使用点号和括号访问嵌套的 JSON 对象：
x = myObj.cars.car2;
//或者：
x = myObj.cars["car2"];

修改值
您能够使用点号来修改 JSON 对象中的任何值：
myObj.cars.car3 = "Mercedes Benz";
您也可以使用括号来修改 JSON 对象中的值：
myObj.cars["car3"] = "Mercedes Benz";

删除对象属性
使用 delete 关键词来删除 JSON 对象的属性：
delete myObj.cars.car1;
```

### JSON 数组：
```
JSON 中的数组几乎与 JavaScript 中的数组相同。在 JSON 中，数组值的类型必须属于字符串、数字、对象、数组、布尔或 null。在 JavaScript 中，数组值可以是以上所有类型，外加任何其他有效的 JavaScript 表达式，包括函数、日期和 undefined。

访问数组值
您可以通过使用索引号来访问数组值：
x = myObj.cars[0];

遍历数组
您可以通过使用 for-in 循环来访问数组值：
for (i in myObj.cars) {
     x  += myObj.cars[i];
}
或者您可以使用 for 循环：
for (i  = 0; i < myObj.cars.length; i++) {
    x  += myObj.cars[i];
}

JSON 对象中的嵌套数组
数组中的值也可以另一个数组，或者甚至另一个 JSON 对象:
myObj =  {
   "name":"Bill Gates",
   "age":62,
   "cars": [
	  { "name":"Porsche",  "models":[ "911", "Taycan" ] },
	  { "name":"BMW", "models":[ "M5", "M3", "X5" ] },
	  { "name":"Volvo", "models":[ "XC60", "V60" ] }
   ]
}
如需访问数组内部的数组，请对每个数组使用 for-in 循环：
for (i in myObj.cars) {
    x += "<h1>" + myObj.cars[i].name  + "</h1>";
    for (j in myObj.cars[i].models) {
         x += myObj.cars[i].models[j];
    }
}

修改数组值
请使用索引号来修改数组：
myObj.cars[1] = "Mercedes Benz";

删除数组项目
请使用 delete 关键词来删除数组中的项目：
delete myObj.cars[1];
```

### JSON PHP:
```
PHP 文件
PHP 提供处理 JSON 的内建函数。通过使用 PHP 函数 json_encode()，PHP 中的对象可转换为 JSON：
<?php
$myObj->name = "Bill Gates";
$myObj->age = 62;
$myObj->city = "Seattle";
$myJSON = json_encode($myObj);
echo $myJSON;
?>

客户端 JavaScript
这是客户端上的 JavaScript，使用 AJAX 调用来请求上例的 PHP 文件,使用 JSON.parse() 把结果转换为 JavaScript 对象：
var xmlhttp = new XMLHttpRequest();
xmlhttp.onreadystatechange = function()  {
    if (this.readyState == 4 && this.status == 200) {
         myObj = JSON.parse(this.responseText);
         document.getElementById("demo").innerHTML = myObj.name;
     }
};
xmlhttp.open("GET", "demo_file.php", true);
xmlhttp.send();
提示：在使用 PHP 函数 json_encode() 时，PHP 中的数组也可以被转换为 JSON。

PHP 数据库
PHP 是服务器端编程语言，应该用于只能由服务器执行的操作，比如访问数据库。想象一下服务器上有一个数据库，包含客户、产品和供应商数据。此刻，您需要请求服务器来获取“客户”表中前十条记录，请使用 JSON.stringify() 将 JavaScript 对象转换为 JSON：
obj = { "table":"customers", "limit":10 };
dbParam = JSON.stringify(obj);
xmlhttp = new XMLHttpRequest();
xmlhttp.onreadystatechange = function() {
     if (this.readyState == 4 && this.status == 200) {
        document.getElementById("demo").innerHTML  = this.responseText;
    }
};
xmlhttp.open("GET",  "demo_json_db.php?x=" + dbParam, true);
xmlhttp.send();
PHP 文件
<?php
header("Content-Type: application/json; charset=UTF-8");
$obj =  json_decode($_GET["x"], false);
$conn = new mysqli("myServer", "myUser", "myPassword", "Northwind");
$result = $conn->query("SELECT name FROM ".$obj->$table." LIMIT ".$obj->$limit);
$outp = array();
$outp = $result->fetch_all(MYSQLI_ASSOC);
echo json_encode($outp);
?>

PHP 方法 = POST
在向服务器发送数据时，通常最好是使用 HTTP POST 方法。如需使用 POST 方法来发送 AJAX 请求，请指定该方法和正确的头部。发送到服务器的数据现在必须是 .send() 方法的参数：
obj = { "table":"customers", "limit":10 };
dbParam = JSON.stringify(obj);
xmlhttp = new XMLHttpRequest();
xmlhttp.onreadystatechange = function() {
     if (this.readyState == 4 && this.status == 200) {
         myObj = JSON.parse(this.responseText);
         for (x in myObj) {
             txt += myObj[x].name + "<br>";
        }
         document.getElementById("demo").innerHTML = txt;
    }
};
xmlhttp.open("POST", "demo_json_db.php", true);
xmlhttp.setRequestHeader("Content-type", "application/x-www-form-urlencoded");
xmlhttp.send("x=" + dbParam);
提示：PHP 文件中的唯一不同是获取被传输数据的方法（使用 $_POST 而不是 $_GET）。
```

### JSONP:
```
JSONP 是一种无需考虑跨域问题即可传送 JSON 数据的方法。JSONP 不使用 XMLHttpRequest 对象。JSONP 使用 <script> 标签取而代之。

JSONP 简介
JSONP 指的是 JSON with Padding。从另一个域请求文件会引起问题，由于跨域政策。从另一个域请求外部脚本没有这个问题。JSONP 利用了这个优势，并使用 script 标签替代 XMLHttpRequest 对象:
<script src="demo_jsonp.php">

Server 文件
服务器上的文件在函数调用中封装结果：
<?php
$myJSON = '{ "name":"Bill Gates", "age":62, "city":"Seattle" }';
echo "myFunc(".$myJSON.");";
?>
结果返回对名为 "myFunc" 的函数的调用，其中的 JSON 数据为参数。请确保客户端存在该函数。

JavaScript 函数
函数 "myFunc" 位于客户端，用于处理 JSON 数据：
function myFunc(myObj)  {
    document.getElementById("demo").innerHTML =  myObj.name;
}

创建动态脚本标签
上例会在页面加载时执行 "myFunc" 函数，根据您放置脚本标签的位置，这样不很令人满意。Script 只应该在需要时创建,在按钮被点击时创建和插入 <script> 标签：
function clickButton() {
    var s = document.createElement("script");
    s.src = "demo_jsonp.php";
    document.body.appendChild(s);
}

回调函数
如果您无法控制服务器文件，那么如何使服务器文件调用正确的函数呢？有时服务器文件提供回调函数作为参数：PHP 文件会调用您作为回调参数传递的函数：
function clickButton() {
    var s = document.createElement("script");
    s.src = "jsonp_demo_db.php?callback=myDisplayFunction";
    document.body.appendChild(s);
}
```

### jQuery vs JavaScript :
```
jQuery 由 John Resig 于 2006 年创建。它旨在处理浏览器不兼容性并简化 HTML DOM 操作、事件处理、动画和 Ajax。十多年来，jQuery 一直是世界上最受欢迎的 JavaScript 库。但是，在 JavaScript Version 5（2009）之后，大多数 jQuery 实用程序都可以通过几行标准 JavaScript 来解决。

通过 id 来查找 HTML 元素
返回 id="intro" 的元素：
jQuery:var myElement = $("#id01");
JavaScript:var myElement = document.getElementById("id01");

通过标签名来查找 HTML 元素
返回所有 <p> 元素：
jQuery:var myElements = $("p");
JavaScript:var myElements = document.getElementsByTagName("p");

通过类名来查找 HTML 元素
返回 class="intro" 的所有元素：
jQuery:var myElements = $(".intro");
JavaScript:var myElements = document.getElementsByClassName("intro");

通过 CSS 选择器查找 HTML 元素
返回包含 class="intro" 的所有 <p> 元素的列表：
jQuery:var myElements = $("p.intro");
JavaScript:var myElements = document.querySelectorAll("p.intro");

设置文本内容
设置 HTML 元素的内部文本：
jQuery:myElement.text("Hello China!");
JavaScript:myElement.textContent = "Hello China!";

获取文本内容
获取 HTML 元素的内部文本：
jQuery:var myText = myElement.text();
JavaScript:var myText = myElement.textContent || myElement.innerText;

设置 HTML 内容
设置元素的 HTML 内容：
jQuery:var myElement.html("<p>Hello World</p>");
JavaScript:var myElement.innerHTML = "<p>Hello World</p>";

获取 HTML 内容
获取元素的 HTML 内容：
jQuery:var content = myElement.html();
JavaScript:var content = myElement.innerHTML;

隐藏 HTML 元素
隐藏一个 HTML 元素：
jQuery:myElement.hide();
JavaScript:myElement.style.display = "none";

显示 HTML 元素
显示一个 HTML 元素：
jQuery:myElement.show();
JavaScript:myElement.style.display = "";

样式化 HTML 元素
更改 HTML 元素的字体尺寸：
jQuery:myElement.css("font-size","35px");
JavaScript:myElement.style.fontSize = "35px";

删除元素
删除 HTML 元素：
jQuery:$("#id").remove();
JavaScript:element.parentNode.removeChild(element);

获取父元素
返回 HTML 元素的父元素：
jQuery:var myParent = myElement.parent();
JavaScript:var myParent = myElement.parentNode;
```

