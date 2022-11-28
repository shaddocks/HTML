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
### 2.1.3 语义相关元素
