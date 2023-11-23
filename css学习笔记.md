# css学习笔记

## css简介

css的唯一作用是让页面变得更加美观

css的规则主要由两部分组成：选择器，一条或多条声明

选择器通常是需要改变样式的html元素

每条声明由一个属性和一个值组成

属性是我们希望设置的样式属性。每个属性有一个值。属性和值用冒号分开

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/77e351fb-f054-4140-b6a2-21abb6803ef4)






## css的引入方式

### 内联样式（行内样式）

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/33dac67c-5072-4660-b3fc-c422d7dd89a5)


内联样式可以对**单个标签**更改属性

这种方式缺乏整体性和规划性，不利于维护





### 内部样式

在head标签内部使用style标签定义内部样式表

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/003c800c-d756-4dba-bbda-a8047490edf9)


内部样式可以对**单个页面**内所有**同名标签**更改属性

这种方式在**单个页面**内的css代码具有统一性和规划性，便于维护，但是在**多个页面**之间容易混乱



### 外部样式

通过单独一个css文件，将需要改变的样式表写出

然后在每个需要改变的html页面文件中，在其head文件中link该css文件，这样就可以通过一个改变文件从而改变多个站点的美观

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/8786cf01-2911-4b21-b2c9-7d4aa4629dd1)






## 选择器

### 全局选择器

可以和任何元素匹配，**优先级最低**，一般做**样式初始化**

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/97095765-5d62-4ea3-89b3-0c305611c655)




### 元素（标签）选择器

html中所有元素如`<p> <a> <img> <div>`等

标签选择器通常描述的都是一个页面上同一个标签的共性，无法描述某一个标签的个性

比如我想在页面上实现这一段话

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/3b93b43b-1c8d-42b8-bdfd-4f0faa53af48)


很明显这段话作为一个段落，我们如果直接对`<p>`更改属性，整句话都会变成红色。但是如果我们在`<p>`标签中给css 加上一个`<span>`标签，任何我们对`<span>`标签更改属性就可以实现了，如下

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/39bb7b96-9bb6-4925-bc4d-f2b267579542)




### 类选择器

规定使用`.`来定义，针对想要的所有标签使用

如下

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/761301e3-2961-4769-bbbf-c85242694560)


我们给第三个`<p>`标签加上一个class属性，任何我们在`<style>`中针对`jsss`使用类选择器，就可以实现对于同样的标签，我们只针对某一个改变某个属性

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/5f377a26-93c0-4bb4-9507-6e430bd54b95)






### ID选择器

针对某一个特定的标签使用，只能使用一次。css中的id选择器用**`#`**定义

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/d2386a74-4f5b-4466-bce7-327c007bc75c)


使用起来和类选择器相似，区别在于ID选择器只能使用一次，而类选择器可以重复使用

### 选择器的优先级

行内样式>ID选择器>类选择器>元素选择器





## 字体属性

### color

规定文本颜色

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/3ca96ecd-6139-4156-9268-9557b6ad4cc5)




### font-size

设置文本大小

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/e123fadb-26a8-4375-9547-2ff7a25b0a21)




### font-weight

设置文本粗细

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/e2abc182-9281-4ad1-ab25-29986b4b4b3d)




### font-style

指定文本的文字样式

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/49269ec2-8163-46b1-9674-45aa7d427ab5)




### font-family

font-family属性指定一个元素的字体

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/55d320ed-ae4c-4a6d-bffc-fd557c5519a0)




## 背景属性

### background-color

设置背景颜色

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/51a280fc-093b-47e9-b46b-27c16b75b4a4)




### background-image

设置元素的背景图片

元素的背景是元素的总大小，包括填充和边界（不包括外边距）。默认情况下background-image属性放置在元素的左上角，如果图像不够大的话会在垂直和水平方向平铺图像，如果图像大小超过元素大小从图像的左上角显示元素的小的那部分

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/ec616452-b985-4380-9acd-858a369538a2)




### background-repeat

设置如何平铺背景图像

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/1e18c0de-1346-41bf-b910-31066260316b)




### background-size

设置背景图像大小

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/ca749fdd-5cc0-43fe-9bf8-ad044b4bd6c5)


cover会填满整个容器，但是会对图片有切割；contain不会对图片进行切割，但不一定能够填满整个容器





### background-position

该属性设置背景图像的起始位置，其默认值是：0% 0%	

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/15a99154-1a3b-43d2-97b3-8f64824c8fda)




## 文本属性

### text-align

指定元素文本的水平对齐方式

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/ced0f307-a2e1-4caf-bd0f-90f5fa710c45)




### text-decoration

该属性规定添加到文本的修饰，下划线，上划线，删除线等等

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/cf7ac1b9-d9f0-4979-8b73-209c8bfe1af7)




### text-transform

该属性控制文本的大小写

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/1d16b2f0-d5cb-4975-86d8-7cb4b636ed27)




### text-indent

该属性规定文本块中首行文本的缩进

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/96ffe5ab-213a-4d65-b189-579dc5b255b2)




## 表格属性

### 表格边框

指定css表格边框，使用border属性

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/317c371a-1fb2-4669-9a90-5c2a54f32bfd)




### 折叠边框

border-collapse属性设置表格的边框是否被折叠成一个单一的边框或隔开



![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/329f2ed1-d8a0-430e-ab34-e23b283a3d11)




### 表格宽度和高度

width和height属性定义表格的宽度和高度

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/45b7e69d-e4f5-439e-99ea-225fd47664a6)




### 表格文字对齐

表格中的文本对齐和垂直对齐属性

text-align属性设置水平对齐方式，向左，或中心

```css
td {text-align:right;}
```

垂直对齐属性设置垂直对齐

```css
td{height:50px;vertical-align:bottom;}
```



### 表格填充

如果在表的内容中控制空格之间的边框，应使用td和th元素的填充属性

```css
td{padding:20px;}
```

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/282181ea-e38e-450e-9fd6-033fb456fc44)


![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/450eeb20-4bba-41b0-bb26-b3d63bf209ae)






## 关系选择器

### 后代选择器

**定义**

选择所有被E包含的F元素

**语法**

```css
E F{}
```

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/778e07f4-8549-4710-9728-d814d64ebdc5)


![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/5935b142-d155-4176-bfc2-4f97b5e4c449)




### 子代选择器

**定义**

选择所有作为E元素的**直接子元素**F，对更深一层的元素不起作用

**语法**

```css
E>F{}
```

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/557f6806-42a8-4c6a-b8ef-cafbfca6bb1e)




### 相邻兄弟选择器

**定义**

选择**紧跟**E元素后的F元素，用加号表示，选择相邻的第一个兄弟元素，**只能向下选择**

**语法**

```css
E+F{}
```

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/d76b189e-f4f6-4f4c-bc19-ce4ea1365155)






### 通用兄弟选择器

**定义**

选择E元素后的所有兄弟F元素，作用于多个元素，用~隔开

**语法**

```css
E~F{}
```

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/0b756a00-f309-47bd-a57e-c56a2e3fe0f2)




## css盒子模型（Box model）

### 概念

所有html元素都可以看成一个盒子，在css中，“box model”这一术语是用来设计和布局时使用

css盒模型本质上是一个盒子，封装周围的html元素，它包括：

外边距（margin），边框（border），内边距（padding）和实际内容（content）

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/99cd0a9e-052f-40ec-ad7c-f0d2d2180f57)


![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/1702c704-e88c-4da4-8aae-bb31b7aea1ea)


![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/b5513f02-ba5c-4094-8447-7df985b4b910)




## 弹性盒子模型（flex box）

### 定义

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/4e56a3cc-5add-4d43-94ab-69def3c07f84)




### css3弹性盒内容

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/d9cca7f7-ad84-49b8-9bf8-d14ee66f53f3)




### 父元素上的属性

#### display属性

`display：flex；`开启弹性盒

`display：flex`属性设置后子元素默认水平排列



#### flex-direction

**定义**

flex-direction属性指定了弹性子元素在父容器中的位置

**语法**

```css
flex-direction : row | row-reverse | column | column-reverse
```

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/85b1763b-8bf0-45fb-bcb6-23c3bc735515)




#### justify-content属性

**定义**

内容对齐属性（justify-content）属性应用在弹性容器上，把弹性项沿着弹性容器的主轴线（main axis）对齐

**语法**

```css
justify-content: flex-start | flex-end | center
```

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/9cab2899-9014-4266-a825-3209edeb6d32)




#### align-items属性

**定义**

`align-items`设置或检索弹性盒子元素在侧轴（纵轴）方向上的对齐方式

**语法**

```css
align-items: flex-start | flex-end | center
```

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/9563b90a-7f99-470b-aee5-734cd45ad56e)



### 子元素上的属性

#### flex

`flex`根据弹性盒子元素所设置的扩展因子作为比率来分配剩余空间

默认为0，即如果存在剩余空间，也不放大

如果只有一个子元素设置，那么按扩展因子转换的百分比对其分配剩余空间。0.1即10%，1即100%，超出按照100%算

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/4c00c8f8-8f64-4441-b450-80a7e9565449)






## 文档流

### 文档流是什么？

文档流是文档中可显示对象在排列时所占用的位置/空间

例如：块元素自上而下摆放，内联元素，从左到右摆放

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/a58170a2-f2e8-413f-82c3-e0d82a261016)




### 文档流产生的问题

#### 高矮不齐，底边对齐

例如![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/94321074-67dc-4fed-b88a-81f8da13104e)


这就是大小不同时，他会自动从底边对齐



#### 空格折叠

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/e7ac43e1-d78b-4cac-8bec-88ae918c30ac)




#### 元素之间有空隙

```css
<span>哈          哈哈</span>
    <img src="mn.webp" alt="">
    <img src="mn.webp" alt="">
```

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/8516660c-a5f6-4290-95ad-9aecb68753ca)




#### 脱离文档流

使一个元素脱离文档流有三种方法

1. 浮动
2. 绝对定位
3. 固定定位



## 浮动

### 定义

`float`属性定义元素在哪个方向浮动，任何元素都可以浮动

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/242775a4-195b-4f15-90f3-372244d33123)




### 浮动的原理

1. 浮动以后使元素脱离了文档流
2. 浮动只有左右浮动，没有上下浮动



### 元素向左浮动

脱离文档流之后，元素相当于在页面上增加一个浮层来放置内容。此时可以理解为有两层页面，一层是底层的原页面，一层是脱离文档流的上层页面，所以会出现折叠现象

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/ad126433-4e08-4966-84e7-280b2db5f9f6)


![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/643c82aa-24fe-447e-819c-1a77885549b3)


![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/84004894-234d-4b2e-9203-5300a114fc63)


![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/3a6b99fc-3d62-4767-bbd7-31afc56fecc2)

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/78a58b84-b94f-4ec7-a97a-2a1607c58591)


![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/15bde92a-993e-47e3-881b-7b144bf1208f)

元素向右浮动于向左类似



### 所有元素向左浮动

当所有元素同时浮动的时候，会变成水平摆放，向左或向右

![image](https://githubfast.com/Bulonte/Tasks/assets/149052453/3e031a51-aef9-4bf6-baff-999b9708dc70)

## 清除浮动

### 浮动副作用

当元素设置float浮动后，该元素就会脱离文档流并向左或向右移动

1. 浮动元素会造成父元素高度塌陷
2. 后续元素会受到影响

![image-20231122163726891](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231122163726891.png)

no float的情况

![image-20231122163848320](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231122163848320.png)

float 的情况

很明显的看到container那个盒子消失了，借助开发者工具![image-20231122164115552](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231122164115552.png)

我们可以很容易的看到这个container盒子是存在的，但是他的高度变为零了。这就时由浮动造成的父元素高度塌陷问题



### 解决方案

1. 给父元素设置高度
2. 受影响的元素增加clear属性
3. overflow清除浮动
4. 伪对象方式



#### 父元素设置高度

如果父元素塌陷，可以给父元素设置高度，撑开元素本身大小

![image-20231122220929792](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231122220929792.png)



#### 受影响的元素增加clear属性

![image-20231122223911109](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231122223911109.png)

![image-20231122223950135](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231122223950135.png)



#### overflow清除浮动

![image-20231122224434333](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231122224434333.png)





#### 伪对象方式

![image-20231122224629371](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231122224629371.png)

![image-20231122225028627](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231122225028627.png)





## 定位

### 定义

`position`属性指定了元素的定位类型

![image-20231122232053136](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231122232053136.png)

其中，**绝对定位和固定定位会脱离文档流**

设置定位之后：可以使用四个方向值进行调整位置：`left`,`top`,`right`,`bottom`



### 相对定位

![image-20231123090207498](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231123090207498.png)

![image-20231123090235357](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231123090235357.png)



### 绝对定位

![image-20231123093305673](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231123093305673.png)



![image-20231123094130210](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231123094130210.png)





### 固定定位

![image-20231123093928338](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231123093928338.png)

固定定位与绝对定位的区别在于：绝对定位会随着页面滑动而滑动，但是固定定位**永远固定不动**



### Z-index

`Z-index`属性设置元素的堆叠顺序。拥有更高堆叠的元素总是会处于堆叠顺序较低的元素的前面

![image-20231123094950732](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231123094950732.png)

![image-20231123095019739](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231123095019739.png)





## css3常用新特性

### 圆角

![image-20231123095318800](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231123095318800.png)

![image-20231123095607965](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231123095607965.png)





### 阴影

​	box-shadow向框添加一个或多个阴影。

![image-20231123095823051](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231123095823051.png)

![image-20231123100231612](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231123100231612.png)



### 动画

动画是使元素从一种样式逐渐变化为另一种样式的效果

我们可以改变任意多的样式任意多的次数

用百分比来规定变化发生的时间，或用关键词`from`和`to`，等同于0%和100%

0%是动画的开始，100%是动画的完成。





#### 创建动画

使用**@keyframes**规则，我们可以创建动画

![image-20231123100954976](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231123100954976.png)





#### 使用动画

我们使用animation来执行动画

![image-20231123101241806](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231123101241806.png)

![image-20231123101317717](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231123101317717.png)

![image-20231123101347199](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231123101347199.png)





### 

 



### 

 
