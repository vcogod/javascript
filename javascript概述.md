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
 * document.documentElementById()
 * document.documentElementsByClassName()[]
 * document.documentElementsByTagName()[]


### 筛选元素
 * el.parentNode
 * el.childNode
 * el.firstNode
 * el.lastNode
 * el.nextNode

### 操作样式
 * el.style.color="red"
 * el.style[color]="red"

### 对位置信息
 * document.documentElement.clientWidth;
 * document.documentElement.clientHeight;
 * obj.offsetWidth


### 属性操作

### 节点操作

### 获取元素信息


### 其他
