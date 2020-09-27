**JavaScript的特殊关键词**

![img](https://api.sololearn.com/DownloadFile?id=2741)

**反斜杠转义特殊字符**

![img](https://api.sololearn.com/DownloadFile?id=2786)

**运算符**

![img](https://api.sololearn.com/DownloadFile?id=2745)

自增和自减

![img](https://api.sololearn.com/DownloadFile?id=2746)

**赋值运算符**

![img](https://api.sololearn.com/DownloadFile?id=2747)

**比较运算符**

![img](https://api.sololearn.com/DownloadFile?id=2748)

==  和===的区别

“=="不仅仅是值之间的比较,也是类型之间的比较

‘===‘仅是值之间的比较,也是类型之间的比较,

**逻辑运算符**

&&   与

||    或

1      非

条件三元运算符

```javascript
var isAdult = (age < 18) ? "Too young": "Old enough";
```



**document和alert的执行顺序问题**

alert会阻塞线程。实际上.write已经执行，只是浏览器还没渲染，这种情况下，有办法先让write执行结果显示。

解决方案

```markdown
想实现“先document.write，再alert”。这里提供下思路：
1>主线程跑document.write() ,然后利用setTimeOut() 定时0。5秒后执行alert();这个方法是线程不可控的 
2>利用promise强制执行document.write()完之后，再在then 方法内执行 alert
```

**switch**

| 语句     | If 语句                  | Switch 语句                      |
| -------- | ------------------------ | -------------------------------- |
| 结构     | 通过嵌套结构实现多重分支 | 专为多重分支设计                 |
| 条件     | 可以测试多个条件表达式   | 仅能测试一个条件表达式           |
| 逻辑关系 | 可以处理复杂的逻辑关系   | 仅能处理多个枚举的逻辑关系       |
| 数据类型 | 可以适用任何数据类型     | 仅能应用整数、枚举、字符串等类型 |

相对而言，下面情况更事宜选用 switch 语句。

- 枚举表达式的值。这种枚举是可以期望的、平行的逻辑关系。
- 表达式的值具有离散性，是不具有线性的非连续的区间值。
- 表达式的值是固定的，不会动态变化。
- 表达式的值是有限的，不是无限的，一般应该比较少。
- 表达式的值一般为整数、字符串等简单的值。


下面情况更事宜用 if 语句。

- 具有复杂的逻辑关系。
- 表达式的值具有线性特征，去对连续的区间值进行判断。
- 表达式的值是动态的。
- 测试任意类型的数据。

default关键词相当与if……else中的else

在两者皆可的情况下考虑时间复杂度时选择switch，考虑空间复杂度时考虑if……else



**函数的参数超过定义**

If you pass more arguments than are defined, they will be assigned to an array called arguments. They can be used like this: arguments[0], arguments[1], etc.



If a function is called with missing arguments (fewer than declared), the missing values are set to undefined, which indicates that a variable has not been assigned a value.



**JavaScript弹窗**

```javascript
var user = prompt("Please enter your name");
alert(user);
```

```javascript
var result = confirm("Do you really want to leave this page?");
if (result == true) {
  alert("Thanks for visiting");
}
else {
  alert("Thanks for staying with us");
}
```

**JavaScript数学对象**![img](https://api.sololearn.com/DownloadFile?id=2769)![img](https://api.sololearn.com/DownloadFile?id=2767)

**JavaScript时间对象**

![img](https://api.sololearn.com/DownloadFile?id=2772)

**DOM中获取要素的主要方式**

//finds element by id
document.**getElementById**(id) 

//finds elements by class name
document.**getElementsByClassName**(name) 

//finds elements by tag name
document.**getElementsByTagName**(name)

**DOM中选择节点的方式**

element.**childNodes** returns an array of an element's child nodes.
element.**firstChild** returns the first child node of an element.
element.**lastChild** returns the last child node of an element.
element.**hasChildNodes** returns true if an element has any child nodes, otherwise false.
element.**nextSibling** returns the next node at the same tree level.
element.**previousSibling** returns the previous node at the same tree level.
element.**parentNode** returns the parent node of an element.



**修改DOM过程中创建的对象**



**console**

**1、console.log** 用于输出普通信息

**2、console.info** 用于输出提示性信息

**3、console.error**用于输出错误信息

**4、console.warn**用于输出警示信息



**event**

![img](https://api.sololearn.com/DownloadFile?id=2777)

**window.onload**   可用于在加载整个页面后运行设置的代码



**DOM事件处理顺序**

冒泡，例如：先处理事件直接发生的元素，再层层处理外部元素



捕获，由外向内处理



**ES6**

var 作用域为全局

let 作用域仅为当前块   比较合适的应用场景 for循环中作为变化的对象

const 的作用域与let相同，但是一但定义了该变量不可变

传统JavaScript和ES6两种以字符串**输出对象值的写法**

```javascript
let name = 'David';
let msg = 'Welcome ' + name + '!';
console.log(msg);
```

```javascript
let name = 'David';
let msg = `Welcome ${name}!`;
console.log(msg);
```

**for 的写法** #类似于python中的for i in list i直接时列表中的对象

```javascript
let list = ["x", "y", "z"];
for (let val of list) {
  console.log(val);
}
```

**函数的新的建立方式**                  #可读性感觉差了好多

```javascript
function add(x, y) {
  var sum = x+y;  
  console.log(sum);
}
```

```javascript
const add = (x, y) => {
  let sum = x + y;  
  console.log(sum);
}
```

==**ES6 对于对象的扩展**==

```javascript
//1.对象的属性简写: 当对象的属性名和属性值（变量）名称一致，可省略赋值
    //2.对象的方法简写：
    let name = "jack";
    let age = 22;

    let obj = {
        name,
        age,
        walk: function () {
            console.log(this.name + " is walk");
        },
        say() {
            console.log(this.name + ` say`);
        }
    }
    
```

**通过俩对象定义新对象**

let newStudent = **Object.assign**({}, person, student);



**promises异步编程的概念**


**取元素的方法**
let listItem = this.parentNode;

