# 第二章
## 2.1 HTML5保留的基本元素
### 2.1.1 基本元素
&emsp;&emsp;HTML文档是一份结构化的文档，HTML文档的根元素总是<html.../>元素，
该元素内通常包含<head.../>和<body.../>两个子元素。这三个元素定义了HTML文档的基本结构。

&emsp;&emsp;HTML5保留的基本元素有如下几个： 
- \<!--...-->: 定义注释。
- \<html>: HTML5的根元素。
- \<head>: 用于定义和HTML5文档的页面头部分。
- \<title>: 用于定义页面标题。
- \<body>: 用于定义页面主体部分，该元素可以指定id, class, style
等通用属性，还可以指定onload, onunload,onclick等事件属性，
这些属性用于自动JavaScript脚本。
- \<h1>到\<h6>: 定义标题一到标题六。
- \<p>: 定义段落。该元素可以指定id, class, style, dir, title,
等通用属性，还可以指定onclick等事件属性。<font color=red size=2>(几乎所有
的HTML元素都可以指定id, class, style, dir, title等通用属性，
其中id属性用于为HTML元素指定一个唯一标识，class和style属性是
CSS样式相关属性。)</font>
- \<br>: 插入一个换行。该元素可以指定id, class, style
等通用属性。
- \<hr>: 定义一个水平线。该元素可以指定id, class, style
等通用属性，还可以指定onclick等各种事件属性。
- \<div>: 定义文档中的节。该元素可以指定id, class, style, 
dir, title等通用属性，还可以指定onclick等各种事件属性。
- \<span>: 与\<div>类似，区别是其只表示一段一般性的文本，该元素
包含的文本内容默认不会换行。指定属性同\<div>。

&emsp;&emsp;<span.../>属性, <div../>属性和<p.../>效果类似，均可作为其他内容
的容器-<font color=red>容纳文本和其他内容</font>。在默认情况下，
<span../><font color=red>不会导致换行</font>，
而<div.../>会<font color=red>导致换行</font>，
而<p.../>元素会<font color=red>产生一个段落</font>，
所以段落和段落 之间默认会有更大的间距。

&emsp;&emsp;<span.../>和<p.../>元素<font color=red>只能包含文本，图像，超链接，
文本格式化元素和表单控件元素等内容</font>。<p.../>可包含<span.../>
元素，但<span.../>不能包含<p.../>；<div.../>除了包含以上元素，还可包含
<h1-h6>, <form.../>, <table.../>, 列表项元素和<div...>元素。
<font color=red><div.../>可包含更多内容</font>。

&emsp;&emsp;建议使用<article.../>, <section.../>等替代<div.../>。
### 2.1.2 文本格式相关元素
&emsp;&emsp;下面这些元素让文本内容在浏览器中呈现出特定效果: 

- \<b>: 定义粗体文本。该元素可以自动id, class,style, dir, title等通用属性，还可以指定onclick等各种事件属性。
- \<i>: 定义斜体文本。该元素可以自动id, class,style, dir, title等通用属性，还可以指定onclick等各种事件属性。
- \<em>: 定义强调文本，实际效果和斜体文本差不多。该元素可以自动id, class,style, dir, title等通用属性，还可以指定onclick等各种事件属性。
- \<strong>: 定义粗体文本。该元素可以自动id, class,style, dir, title等通用属性，还可以指定onclick等各种事件属性。
- \<small>: 定义小号字体文本。该元素可以自动id, class,style, dir, title等通用属性，还可以指定onclick等各种事件属性。
- \<sup>: 定义上标文本。该元素可以自动id, class,style, dir, title等通用属性，还可以指定onclick等各种事件属性。
- \<sub>: 定义下标文本。该元素可以自动id, class,style, dir, title等通用属性，还可以指定onclick等各种事件属性。
- \<bdo>: 定义文本显示的方向。该元素可以自动id, class,style, dir, title等通用属性，还可以指定onclick等各种事件属性。除此之外，该元素应该指定dir属性，该属性值只能是ltr或者rtl，用于指定文本的排列方向。

上面这些文本格式化元素能包含文本、图像、超链接、文本格式化元素和表单控件元素等。除此之外还可以与<span>相互包含。

### 2.1.3 语义相关元素
&emsp;&emsp;如下语义相关元素:

- \<abbr>: 用于表示一个缩写。使用该元素时通常建议指定title属性，该属性用于指定该缩写所代表的全称。
- \<address>: 用于表示一个地址。浏览器通常用斜体字显示。
- \<blockquote>: 用于定义一段长的引用文本。浏览器使用缩进的方式显示这段被引用文本。可指定cite属性，该属性用于指定该引用文本所引用的网址URL或出处。
- \<q>: 用于定义一段短的引用文本。浏览器会为这段文本添加引号。与<blockquote.../>类似，通常不换行，短文本。
- \<cite>: 用于表示作品(书，电影)的标题。浏览器通常会用斜体显示。
- \<code>: 用于表示一段计算机代码。
- \<dfn>: 用于定义一个专业术语。浏览器通常会用粗体或斜体显示。
- \<del>: 定义文档中被删除的文本。浏览器通常会以中画线形式显示。
- \<ins>: 定义文档中插入的文本。浏览器通常会以下画线形式显示。
<del.../>和<ins.../>通常结合使用，表示文档被修订的效果，而且使用这两个元素时都可以指定如下两个元素。
<font color=red>cite</font>-该属性值为一个URL，该URL对应的文本解释了文本被删除或插入的原因。
<font color=red>datetime</font>-定义文本被删除或插入的日期，时间。
- \<pre>: 用于表示该元素所包含的文本已经进行了"预格式化"。即该元素所包含的文本中的空格，回车，Tab和其他格式字符都会保留下来，但浏览器会处理该元素内大部分HTML元素。
- \<samp>:用于定义示范文本内容。
- \<kbd>: 用于定义键盘文本。该元素用于表示文本是通过键盘输入的。通常在计算机使用文档，使用说明中会经常使用该元素。
- \<var>: 用于表示一个变量。浏览器通常会用斜体字显示。
