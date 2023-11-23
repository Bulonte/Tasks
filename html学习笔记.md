# html学习笔记

## 基础知识

```
<html> 与 </html> 之间的文本描述网页
<body> 与 </body> 之间的文本是可见的页面内容
<h1> 与 </h1> 之间的文本被显示为标题
<p> 与 </p> 之间的文本被显示为段落
```



## html 链接

![image-20231116221615626](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231116221615626.png)

```
HTML 链接是通过 <a> 标签进行定义的。
```

![image-20231114165005185](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231114165005185.png)



在 href 属性中指定链接的地址

![image-20231116222337841](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231116222337841.png)









## html水平线

```
<hr /> 标签在 HTML 页面中创建水平线。

hr 元素可用于分隔内容。
```

![image-20231116180444392](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231116180444392.png)

## html注释

可以将注释插入 HTML 代码中，这样可以提高其可读性，使代码更易被人理解。浏览器会忽略注释，也不会显示它们。

注释是这样写的：

![image-20231114170311204](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231114170311204.png)



## html折行

```
如果您希望在不产生一个新段落的情况下进行换行（新行），请使用 <br /> 标签：
```

![image-20231114223913386](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231114223913386.png)



## html 的style

background-color 属性为元素定义了背景颜色：

```
<html>

<body style="background-color:yellow">
<h2 style="background-color:red">This is a heading</h2>
<p style="background-color:green">This is a paragraph.</p>
</body>

</html>
```

效果

![image-20231116165110210](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231116165110210.png)



## html图片

![image-20231116181210898](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231116181210898.png)

![image-20231116181714331](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231116181714331.png)

![image-20231116181759698](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231116181759698.png)

！！！**图片文件和html文件必须在同一个文件夹内**

**如果不在同一个文件夹内，则需要用图片文件的绝对地址，使得代码可以调用该图片**

![image-20231116215943697](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231116215943697.png)



## html文本

![image-20231117135403080](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231117135403080.png)

![image-20231117140001429](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231117140001429.png)

 



## html列表

### 有序列表

![image-20231117141247886](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231117141247886.png)

![image-20231117141946864](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231117141946864.png)

![image-20231117142109768](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231117142109768.png)

### 无序列表

![image-20231117142728189](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231117142728189.png)

![image-20231117142808442](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231117142808442.png)

![image-20231117143140105](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231117143140105.png)

![image-20231118141633425](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231118141633425.png)





## html表格

### 表格基础知识

![image-20231118142651998](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231118142651998.png)

![image-20231118142433300](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231118142433300.png)

！！！**td和tr标签必须在table标签内部使用**

![image-20231118142758102](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231118142758102.png)

![image-20231118143227782](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231118143227782.png)

### 表格的合并

水平合并：colspan

竖直合并：rowspan 

![image-20231118165938878](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231118165938878.png)





## html表单

### 表单是什么？

​	![image-20231118170403471](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231118170403471.png)

### 表单的属性

![image-20231118170432780](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231118170432780.png)

### 表单元素

![image-20231118171103801](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231118171103801.png)

**表单标签：form**

**表单域：input**

**表单按钮：button**

![image-20231118171712001](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231118171712001.png)

![image-20231118172154114](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231118172154114.png)

![image-20231118172331698](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231118172331698.png)

![image-20231118172735353](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231118172735353.png)



## 块级元素与内联元素的区别

![image-20231119204023067](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231119204023067.png)

![image-20231119204046658](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231119204046658.png)



## H5新标签

![image-20231119205637956](C:\Users\钟佑安\AppData\Roaming\Typora\typora-user-images\image-20231119205637956.png)

！！！**2014年之前的浏览器不支持H5新标签**