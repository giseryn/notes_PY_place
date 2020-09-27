**<!DOCTYPE html>的含义**
html5标准网页声明,全称为Document Type HyperText Mark-up Language，
意思为文档种类为超文本标记性语言或超文本链接标示语言
作用：声明文档的解析类型(document.compatMode)，避免浏览器的怪异模式。
使用：<!DOCTYPE html>

**如何解决页面乱码问题？**　　
在head节点加入此行标记，把字符声明为UTF-8
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />  
解释这句：
http-equiv="Content-Type" 表示描述文档类型
content="text/HTML;  文档类型，这里为html,如果JS就是text/javascript，
charset=utf-8 页面字符集，编码，eg:gb2312,iso-8859-1,utf-8

**img支持的文件格式**
png、jpg、gif
展示色彩丰富的高品质图片，使用jpg格式，但是体积较大；
png格式，体积较小且支持保存透明背景；
展示动画图片，可以使用gif图片格式。

**空内容**
某些 HTML 元素具有空内容（empty content）
空元素在开始标签中进行关闭（以开始标签的结束而结束）
大多数 HTML 元素可拥有属性

**换行**
<br/>

**标签属性**
属性值应该始终被包括在引号内。双引号是最常用的，
不过使用单引号也没有问题。
background-color 属性为元素定义了背景颜色：
font-family 定义元素中文本的字体系列
color       定义元素中文本的颜色
font-size   定义元素中文本的字体尺寸
text-align  属性规定了元素中文本的水平对齐方式：

**水平线**
<hr/>

**文本格式化**

标签	描述
<b>	定义粗体文本。<br/>
<big>	定义大号字。<br/>
<em>	定义着重文字。<br/>
<i>	 定义斜体字。<br/>
<small>	定义小号字。<br/>
<strong>定义加重语气。<br/>
<sub>	定义下标字。<br/>
<sup>	定义上标字。<br/>
<ins>	定义插入字。<br/>
<del>	定义删除字<br/>
#
<code>	定义计算机代码。

<kbd>	定义键盘码。

<samp>	定义计算机代码样本。

<tt>	定义打字机代码。

<var>	定义变量。

<pre>	定义预格式文本。</pre>

<abbr>	定义缩写。

<acronym>	定义首字母缩写。

<address>	定义地址</address>

<bdo>	定义文字方向。

<blockquote>	定义长的引用。</blockquote>

<q>	定义短的引用语。

<cite>	定义引用、引证。

<dfn>	定义一个定义项目。

**引用**

HTML &lt;q&gt; 用于短的引用

HTML &lt;blockquote&gt;用于长引用的

用于缩略词的 &lt;abbr&gt;



**在HTML中打出<>等HTML关键词的方法**
<p>＆lt代表<,＆gt代表></p>

**语义化：网页划分逻辑单元**
&lt;div&gt;
&lt;header&gt;页首
&lt;footer&gt; 页脚
&lt;section&gt;页面主题
&lt;aside&gt; 侧栏
&lt;nav&gt; 导航栏

一般是&lt;header&gt;和&lt;footer&gt;作为头尾，在section中用&lt;div&gt;分区

**HTML中空格**

这里有&nbsp;一个空格

**双向重写**
用于双向重写的 HTML <bdo>
HTML <bdo> 元素定义双流向覆盖（bi-directional override）。
<bdo> 元素用于覆盖当前文本方向：

ltr，rtl定义文字方向

**邮件链接**
mailto:邮箱？cc=抄送&bcc=抄送二号&subject=主题&body=信的内容

**设置图片和文本的位置 对齐方式（align）**
botton 默认
middle
top

right left

**图片无法显示时显示文本**
alt="向左转" 关键词

**定义图片中的可点区域**
area
可调参数
coords	坐标值	定义可点击区域（对鼠标敏感的区域）的坐标。
href	URL	定义此区域的目标 URL。
nohref	nohref	从图像映射排除某个区域。
shape           定义区域形状
target          规定何处打开目标url

**空格占位符**
 &nbsp ;

**单元格参数**
 colspan="2" #横跨两列
 rowspan="2" #横跨两行
 bgcolor="red" #设置背景色
 background="/i/eg_bg_07.gif"  #设置背景图片
 cellspacing="10"  #每个单元格之间的距离
 align="left"  #设置表格内内容的位置
 <thead>	#定义表格的页眉。
 <tbody>	#定义表格的主体。
 <tfoot>	#定义表格的页脚。
 <col>	#定义用于表格列的属性。
 <colgroup>	#定义表格列的组。

 **列表**
 ul 无序列表
 type="disc"    #实心圆
 type="disc"    #空心圆
 type="disc"    #实心方块

 ol有序列表
 type 无参1234
      A， a 大小写字母
      
 <ol>	定义有序列表。 </ol>
 <ul>	定义无序列表。 </ul>
 <li>	定义列表项。
 <dl>	定义定义列表。</dl>
 <dt>	定义定义项目。</dt>
 <dd>	定义定义的描述。</dd>

 **网页框架**
 框架结构标签&lt;frameset&gt;
 框架标签（Frame）
 &lt;frame src="frame_a.html"&gt;

 noresize="noresize"。#此参数可以防止用户改变框架大小

 iframe 用于在网页中显示网页


**noscript**
可以在浏览器禁用脚本时显示提示语

**链接跳转还是原窗口打开**
在头文件中设置 base target="_blank" /
或者在跳转语句中设置

**字符实体**

| 空格 | &nbsp;            | &#160;            |         |
| ---- | ----------------- | ----------------- | ------- |
| <    | 小于号            | &lt;              | &#60;   |
| >    | 大于号            | &gt;              | &#62;   |
| &    | 和号              | &amp;             | &#38;   |
| "    | 引号              | &quot;            | &#34;   |
| '    | 撇号              | &apos; (IE不支持) | &#39;   |
| ￠   | 分（cent）        | &cent;            | &#162;  |
| £    | 镑（pound）       | &pound;           | &#163;  |
| ¥    | 元（yen）         | &yen;             | &#165;  |
| €    | 欧元（euro）      | &euro;            | &#8364; |
| §    | 小节              | &sect;            | &#167;  |
| ©    | 版权（copyright） | &copy;            | &#169;  |
| ®    | 注册商标          | &reg;             | &#174;  |
| ™    | 商标              | &trade;           | &#8482; |
| ×    | 乘号              | &times;           | &#215;  |
| ÷    | 除号              | &divide;          | &#247;  |

 

​      
