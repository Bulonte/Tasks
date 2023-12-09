# Markdown学习笔记（常用语法）

## 一.标题语法

标题总共分为六级，用#表示。不同级别标题区别在于大小不同。



## 二. 段落语法

要创建段落，使用空白行将一行或多行文本进行分隔。不要用空格（spaces）或制表符（ tabs）缩进段落。



## 三.换行语法  

在一行的末尾添加两个或多个空格，然后按回车键,即可创建一个换行(`<br>`)。



## 四 .强调语法

### 1.粗体

要加粗文本，在单词或短语的前后各添加两个星号（asterisks）或下划线（underscores）。如需加粗一个单词或短语的中间部分用以表示强调的话，请在要加粗部分的两侧各添加两个星号（asterisks）。

### 2.斜体

要用斜体显示文本，在单词或短语前后添加一个星号（asterisk）或下划线（underscore）。要斜体突出单词的中间部分，请在字母前后各添加一个星号，中间不要带空格。

### 3.又粗又斜体

要同时用粗体和斜体突出显示文本，在单词或短语的前后各添加三个星号或下划线。要加粗并用斜体显示单词或短语的中间部分，请在要突出显示的部分前后各添加三个星号，中间不要带空格。



## 五. 引用语法

### 1.单块引用

要创建块引用，在段落前添加一个 `>` 符号。

### 2.多块引用

块引用可以包含多个段落。为段落之间的空白行添加一个 `>` 符号。（说简单点就是要引用的每一行都加 `> `）

## 3.嵌套块引用

块引用可以嵌套。在要嵌套的段落前添加一个 `>>` 符号。



## 六.列表语法

### 1.有序列表

要创建有序列表，在每个列表项前添加数字并紧跟一个英文句点。数字不必按数学顺序排列，但是列表应当以数字 1 起始。

例如：

1.one

2.two

......

### 2.无序列表

要创建无序列表，在每个列表项前面添加破折号 (-)、星号 (*) 或加号 (+) 。缩进一个或多个列表项可创建嵌套列表。

### 3.在列表中嵌套

要在保留列表连续性的同时在列表中添加另一种元素，将该元素缩进四个空格或一个制表符。



## 七.代码语法（`）

### 1.反引号

要将单词或短语表示为代码，将其包裹在反引号 (```) 中。

### 2.转义反引号

如果你要表示为代码的单词或短语中包含一个或多个反引号，则可以通过将单词或短语包裹在双反引号(````)中。



### 3.代码块

要创建代码块，将代码块的每一行缩进至少四个空格或一个制表符。



## 八.分隔线语法

要创建分隔线，在单独一行上使用三个或多个星号 (`***`)、破折号 (`---`) 或下划线 (`___`) ，并且不能包含其他内容。（为了兼容性，在分隔线的前后均添加空白行。）



## 九. 链接语法

链接文本放在中括号内，链接地址放在后面的括号中，链接title可选。

超链接Markdown语法代码：`[超链接显示名](超链接地址 "超链接title")`

```text
这是一个链接 [Markdown语法](https://markdown.com.cn)。
```



### 1.给链接加Title

链接title是当鼠标悬停在链接上时会出现的文字，这个title是可选的，它放在圆括号中链接地址后面，跟链接地址之间以空格分隔。

```text
这是一个链接 [Markdown语法](https://markdown.com.cn "最好的markdown教程")。
```



### 2.网址和Email地址

使用尖括号可以很方便地把URL或者email地址变成可点击的链接。

```text
<https://markdown.com.cn>
<fake@example.com>
```



### 3.带格式化的链接

[强调](https://markdown.com.cn/basic-syntax/links.html#emphasis) 链接, 在链接语法前后增加星号。 要将链接表示为代码，请在方括号中添加反引号。

```text
I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#code).
```



### 4.引用类型链接

引用样式链接是一种特殊的链接，它使URL在Markdown中更易于显示和阅读。参考样式链接分为两部分：与文本保持内联的部分以及存储在文件中其他位置的部分，以使文本易于阅读。

#### [#](https://markdown.com.cn/basic-syntax/links.html#链接的第一部分格式)链接的第一部分格式

引用类型的链接的第一部分使用两组括号进行格式设置。第一组方括号包围应显示为链接的文本。第二组括号显示了一个标签，该标签用于指向您存储在文档其他位置的链接。

尽管不是必需的，可以在第一组和第二组括号之间包含一个空格。第二组括号中的标签不区分大小写，可以包含字母，数字，空格或标点符号。

以下示例格式对于链接的第一部分效果相同：

- `[hobbit-hole][1]`
- `[hobbit-hole] [1]`

#### [#](https://markdown.com.cn/basic-syntax/links.html#链接的第二部分格式)链接的第二部分格式

引用类型链接的第二部分使用以下属性设置格式：

1. 放在括号中的标签，其后紧跟一个冒号和至少一个空格（例如`[label]:`）。
2. 链接的URL，可以选择将其括在尖括号中。
3. 链接的可选标题，可以将其括在双引号，单引号或括号中。

以下示例格式对于链接的第二部分效果相同：

- `[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle`
- `[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"`
- `[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'`
- `[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)`
- `[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"`
- `[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'`
- `[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles)`

可以将链接的第二部分放在Markdown文档中的任何位置。有些人将它们放在出现的段落之后，有些人则将它们放在文档的末尾（例如尾注或脚注）

## 十.图片语法

要添加图像，请使用感叹号 (`!`), 然后在方括号增加替代文本，图片链接放在圆括号里，括号里的链接后可以增加一个可选的图片标题文本。

插入图片Markdown语法代码：`![图片alt](图片链接 "图片title")`。

对应的HTML代码：`<img src="图片链接" alt="图片alt" title="图片title">`

```text
![这是图片](/assets/img/philly-magic-garden.jpg "Magic Gardens")
```



###  链接图片

给图片增加链接，请将图像的Markdown 括在方括号中，然后将链接添加在圆括号中。

```text
[![沙漠中的岩石图片](/assets/img/shiprock.jpg "Shiprock")](https://markdown.com.cn)
```



#这是一级标题

# 这是一级标题

##这是二级标题

## 这是二级标题

###这是三级标题

### 这是三级标题