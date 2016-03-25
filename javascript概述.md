# javascript概述

##基础逻辑处理部分
 
 >变量 数据类型  (数据存储)
 >分支和循环、运算符    (逻辑操作)
 >函数(对语言的扩展)

###变量类型

```javascript
var a=a; //Number
var a="11"; //String
var a=true; //Boolean
var a=[1,2,3,4]; //Array
var a={a:1,b:2}; //Object
var a=function(){}; //Function
var a=undefined
var a=null

###运算符

+ - * / %   ===  !==  > < <= >=
&&   ||   !    

###分支语句

if()
if() else if()
if() else if()  else if()
swith(x){
	case 1:
	break;
	case 2:
	break;
	default;
	break;
	}

###循环语句

for (var i=0,k=12;i<10;i++){}
while(){}
do{}while()

###函数

function xx(){
	
}
var fn=function(x1,x2){
	//arguments
}
fn(a,b)
function A(b){
	this.x=b
}
A.prototype.console=function(){
	console.log(this.x)
}
var obj=new A(1);
obj.console();
```

//数组的常用方法
//字符串的常用方法
//函数对象中的方法 bind apply call
//对象的增删改查 原型链
//数字对象身上的方法 toFixed()
//Math对象身上的方法


## 针对特定用途的部分
 > 当js来浏览器运行的那一刻
 > 浏览器会创建一个window对象
 > window对象中有很多属性和方法
 > 这些属性和方法不用加 window. 就可以调用

dom对象 dom集合

 ### 选取元素

* var el=document.createElement()
* var el=document.getElementById()
* var el=document.querySelector()  //ie8

* var el=document.getElementsclassName()
* var el=document.getElementsTagName()
* var el=document.getElementsByName()
* var el=document.querySelectorAll()   //ie8
* var el=document.genElementsById()

### 筛选元素
 >父元素
   *el.parentNode
  *el.parentElement
 >子元素
  *el.firstchilds
  *el.firstElementChild
 >兄弟
  *el.nextSibling
  *el.nextElementSibling

  *el.previousSibling
  *el.previousElementSibling

  *el.lastchilds
  *el.lastElementChild

  *el.ChildNodes
  *el.Child
### 对位置信息
 * document.documentElement.clientWidth;
 * document.documentElement.clientHeight;
 * obj.offsetWidth


### 属性操作（Element）

 * el.setAttribute()
 * el.getAttribute()
 * el.removeAttribute()
 * el.hasAttribute()
 * el.ClassName
 * el.id
 * el.ClassList



### 节点操作  (Node)

 * el.appendChild()
 * el.removeChild()
 * el.insertBefor()
 * el.cloneNode()
 * el.replaceChild()  //替换


### 获取元素信息 （HTMLElement）

* el.offseWidth
* el.offseHeight
* el.offsetLeft
* el.offsetTop
* el.offsetParent
* el.getBoundingClieRect()  //计算元素距窗口的

* el.innerHTML


### 操作样式

 * el.style(读取/设置行内样式的值)
 
 el.style.color='red'
### 其他

var obj={
	a:1,
	c:2,
	set c (x) {console.log(111)},
	get c () {return 5;}
}