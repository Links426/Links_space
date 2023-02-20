> 这篇笔记是自己补基础的时候所写的，在刚开始学习js基础的过程中，有很多没有学习到。因此这篇笔记算为自己不会的地方进行补强。

## JavaScript 基础 ，从零开始补基础。

## 1. 初识 JavaScript

### 	1.1 浏览器执行 JS 简介

​		浏览器分为 渲染引擎 和 JS 引擎

> 渲染引擎: 用来解析HTML 和 CSS，俗称内核。例如 Chrome 浏览器里面的 blink，老版本 Chrome 的 WebKit 
>
> JS 引擎: 也称作 JS 解析器。用来读取网页中的 JavaScript 代码，对其处理后运行。比如 chrome 浏览器的 V8 引擎。

​		浏览器本身不会执行JS代码，而是通过内置的JS引擎（解释器）来执行JS代码。JS引擎执行代码时逐行解释每一句源码（转换为机器语言），然后由计算机去执行。所以 JS 语言归为脚本语言，会逐行解释执行

### 	1.2 JS 的 组成

```
1. ECMAScript (JavaScript 语法)
2. DOM (页面文档对象模型) 对页面上的各种元素进行操作（大小、位置、颜色等）
3. BOM (浏览器对象模型) 操作浏览器窗口，比如弹出框、控制浏览器跳转、获取分辨率等
```

### 	1.3 JS 输入输出 语句

```
1. alert(msg) 浏览器弹出警示框
2. console.log(msg) 浏览器控制台打印输出信息
3. prompt(info) 浏览器弹出输入框，用户可以输入
```

​	

## 2. JavaScript 基础语法

### 	2.1 数据类型

#### 		2.3.1 类型分类

```
JavaScript 中 一共有 五种数据类型
1. String（字符串型）
2. Number（数值型）
3. Boolean（布尔型）
4. undefined
5. Null
```

> 这五种类型之外的 都称为 Object，所以总的来看 JS 中 共有六种数据类型

#### 		2.3.2 typeof 运算符

```javascript
// 使用方法：typeof xxx
```

```javascript
console.log(typeof null) // 结果：object
console.log(typeof undefined) // 结果：undefined
```

#### 		2.3.3 String

```
		 String 用于表示一个字符串。
```

​		转义字符 :

```javascript
1. \n 换行
2. \t 制表
3. \b 空格
4. \r 回车
5. \\ 斜杠
6. \' 单引号
7. \" 双引号
```

#### 		2.3.4 Number

```
Number 类型用来表示整数和浮点数
Number 表示的数字大小是有限的，如果超过了这个范围，则会显示 +/- Infinity
```

​		特殊的数字：

```
Infinity: 正无穷
-Infinity: 负无穷
NaN : 非法数字(Not A Number)
```

```javascript
console.log(typeof Infinity) // Number
console.log(typeof NaN) // Number
```

#### 		2.3.5 Boolean

> Boolean布尔型 只能够取 真(true) 和 假(false) ，其他的数不被支持

#### 		2.3.6 Undefined

​		Undefined 类型只有一个值，即特殊的 Undefined 

​		在使用 var 声明变量，但未将其初始化时，这个变量的值就是 undefined

```javascript
var test
console.log(test) // undefined
```

> 使用 typeof 对没有定义和没有初始化的变量 会返回 undefined

```javascript
var test
console.log(typeof test) // undefined
```

