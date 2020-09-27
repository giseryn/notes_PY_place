**CSS选择器**

<ul>派生选择器

</ul>

<ul>id选择器

</ul>

<ul>类选择器</ul>

<ul>属性选择器（适合表单的样式设计）

| 选择器                                                       | 描述                                                         |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [[*attribute*\]](https://www.w3school.com.cn/cssref/selector_attribute.asp) | 用于选取带有指定属性的元素。                                 |
| [[*attribute*=*value*\]](https://www.w3school.com.cn/cssref/selector_attribute_value.asp) | 用于选取带有指定属性和值的元素。                             |
| [[*attribute*~=*value*\]](https://www.w3school.com.cn/cssref/selector_attribute_value_contain.asp) | 用于选取属性值中包含指定词汇的元素。                         |
| [[*attribute*\|=*value*\]](https://www.w3school.com.cn/cssref/selector_attribute_value_start.asp) | 用于选取带有以指定值开头的属性值的元素，该值必须是整个单词。 |
| [[*attribute*^=*value*\]](https://www.w3school.com.cn/cssref/selector_attr_begin.asp) | 匹配属性值以指定值开头的每个元素。                           |
| [[*attribute*$=*value*\]](https://www.w3school.com.cn/cssref/selector_attr_end.asp) | 匹配属性值以指定值结尾的每个元素。                           |
| [[*attribute**=*value*\]](https://www.w3school.com.cn/cssref/selector_attr_contain.asp) | 匹配属性值中包含指定值的每个元素。                           |

**CSS样式**

background-colar #背景色，可以为所有元素设置背景色，这包括 body 一直到 em 和 a 等行内元素。

background-image #背景图像，通过url设置背景



**位置关键词**

top、bottom、left、right 和 center

默认要水平方向关键词和垂直方向关键词，缺乏关键词时默认为居中

百分比，像素值可以混合使用

background-attachment:fixed 可以设置背景位置不随页面滚轮滑动



**文本属性**

text_indent            	#文本缩进（可以通过设置负值实现文本段落悬挂的效果，要针对负缩进设置外边距或内边距）

​									#可以设置长度缩进，百分比缩进（针对父元素大小）

text-align:center  	#文本居中

​								   #对齐属性 left right center

​								   #justify属性可以两端对齐

word-spacing           #可以增加或者减少词与词之间的间隔

letter-spacing           #可以减少或增加字母之间的距离

**text-transform** 设置字符的大小写等属性

- none

- uppercase

- lowercase

- capitalize

  **text-decoration**设置字符的划线

- none          #通过设置使超链接的下划线消失

- underline

- overline

- line-through

- blink

下面的表格总结了 white-space 属性的行为：

| 值       | 空白符 | 换行符 | 自动换行 |
| :------- | :----- | :----- | :------- |
| pre-line | 合并   | 保留   | 允许     |
| normal   | 合并   | 忽略   | 允许     |
| nowrap   | 合并   | 忽略   | 不允许   |
| pre      | 保留   | 保留   | 不允许   |
| pre-wrap | 保留   | 保留   | 允许     |

## CSS 字体属性

| 属性                                                         | 描述                                                   |
| :----------------------------------------------------------- | :----------------------------------------------------- |
| [font-style](https://www.w3school.com.cn/cssref/pr_font_font-style.asp) | 设置字体风格。                                         |
| [font-variant](https://www.w3school.com.cn/cssref/pr_font_font-variant.asp) | 以小型大写字体或者正常字体显示文本。                   |
| [font-weight](https://www.w3school.com.cn/cssref/pr_font_weight.asp) | 设置字体的粗细。                                       |
| [font](https://www.w3school.com.cn/cssref/pr_font_font.asp)  | 简写属性。作用是把所有针对字体的属性设置在一个声明中。 |
| [font-family](https://www.w3school.com.cn/cssref/pr_font_font-family.asp) | 设置字体系列。                                         |
| [font-size](https://www.w3school.com.cn/cssref/pr_font_font-size.asp) | 设置字体的尺寸。                                       |

**CSS链接**

- a:link - 普通的、未被访问的链接
- a:visited - 用户已访问的链接
- a:hover - 鼠标指针位于链接的上方
- a:active - 链接被点击的时刻

#为了使定义生效，a:hover 必须位于 a:link 和 a:visited 之后！！

#为了使定义生效，a:active 必须位于 a:hover 之后！！



**CSS 框模型 (Box Model)** 规定了元素框处理元素内容、内边距、边框 和 外边距 的方式。

**CSS定位方法**  普通流、浮动和绝对定位

相对定位，绝对定位，固定定位

overflow 处理溢出部分，对于溢出部分，处理方式scroll 提供滚动机制，

​				auto 自动处理，hidden 隐藏溢出部分

Z-index 可以设置要素的层级



**要素浮动**

float：方位

clear 可以规定要素的某一方向不存在浮动：只能作用在定义该参数的要素上

即使div1的宽度很小，页面中一行可以容下div1和div2，div2也不会排在div1后边，因为div元素是独占一行的。

 浮动可以理解为让某个div元素脱离标准流，漂浮在标准流之上，和标准流不是一个层次。



**选择器优先级**

内联 > ID选择器 > 类选择器 > 标签选择器。

**对齐**

margin 水平对齐

position 左右对齐



**显示方式**

内联inline

块级block



**透明度**

opacity



**外框和内距**

margin 外边距

padding 内边距



**transition**[https://www.cnblogs.com/xiaohuochai/p/5347930.html]

设置过渡效果的CSS属性名称

transition-duration 过度时间

transition-delay   过渡延迟时间

transition-timing-function 过渡函数

steps(<integer>[,start | end]?) 过渡步数



过渡transition的这四个子属性只有<transition-duration>是必需值且不能为0。其中，<transition-duration>和<transition-delay>都是时间。当两个时间同时出现时，第一个是<transition-duration>，第二个是<transition-delay>；当只有一个时间时，它是<transition-duration>，而<transition-delay>为默认值0

不是所有的CSS样式值都可以过渡，只有具有中间值的属性才具备过渡效果



```
颜色: color background-color border-color outline-color
位置: backround-position left right top bottom
长度: 
    [1]max-height min-height max-width min-width height width
    [2]border-width margin padding outline-width outline-offset
    [3]font-size line-height text-indent vertical-align  
    [4]border-spacing letter-spacing word-spacing
数字: opacity visibility z-index font-weight zoom
组合: text-shadow transform box-shadow clip
其他: gradient
```



**CSS中的简单函数**

| 函数                                                         | 描述                                                         | CSS 版本 |
| :----------------------------------------------------------- | :----------------------------------------------------------- | :------- |
| [attr()](https://www.runoob.com/cssref/func-attr.html)       | 返回选择元素的属性值。                                       | 2        |
| [calc()](https://www.runoob.com/cssref/func-calc.html)       | 允许计算 CSS 的属性值，比如动态计算长度值。                  | 3        |
| [cubic-bezier()](https://www.runoob.com/cssref/func-cubic-bezier.html) | 定义了一个贝塞尔曲线(Cubic Bezier)。                         | 3        |
| [hsl()](https://www.runoob.com/cssref/func-hsl.html)         | 使用色相、饱和度、亮度来定义颜色。                           | 3        |
| [hsla()](https://www.runoob.com/cssref/func-hsla.html)       | 使用色相、饱和度、亮度、透明度来定义颜色。                   | 3        |
| [linear-gradient()](https://www.runoob.com/cssref/func-linear-gradient.html) | 创建一个线性渐变的图像                                       | 3        |
| [radial-gradient()](https://www.runoob.com/cssref/func-radial-gradient.html) | 用径向渐变创建图像。                                         | 3        |
| [repeating-linear-gradient()](https://www.runoob.com/cssref/func-repeating-linear-gradient.html) | 用重复的线性渐变创建图像。                                   | 3        |
| [repeating-radial-gradient()](https://www.runoob.com/cssref/func-repeating-radial-gradient.html) | 类似 radial-gradient()，用重复的径向渐变创建图像。           | 3        |
| [rgb()](https://www.runoob.com/cssref/func-rgb-css.html)     | 使用红(R)、绿(G)、蓝(B)三个颜色的叠加来生成各式各样的颜色。  | 2        |
| [rgba()](https://www.runoob.com/cssref/func-rgba.html)       | 使用红(R)、绿(G)、蓝(B)、透明度(A)的叠加来生成各式各样的颜色。 | 3        |
| [var()](https://www.runoob.com/cssref/func-var.html)         | 用于插入自定义的属性值。                                     | 3        |



**CSS速记属性**

如 [`font`](https://developer.mozilla.org/zh-CN/docs/Web/CSS/font), [`background`](https://developer.mozilla.org/zh-CN/docs/Web/CSS/background), [`padding`](https://developer.mozilla.org/zh-CN/docs/Web/CSS/padding), [`border`](https://developer.mozilla.org/zh-CN/docs/Web/CSS/border), and [`margin`](https://developer.mozilla.org/zh-CN/docs/Web/CSS/margin) 等属性称为速记属性--这是因为它们允许您在一行中设置多个属性值，从而节省时间并使代码更整洁。



**CSS的注释**

```css
/* Handle basic element styling */
```



















