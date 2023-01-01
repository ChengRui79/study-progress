# HTML

## day1

本质：前端代码通过浏览器解析、渲染转换成网页

五大主流浏览器内核（渲染引擎）不同，渲染效果可能略有不同，这就需要一个Web标准

Web标准由html（结构）、css（表现）、js（行为）构成

html（超文本标记语言）

<strong>你猜，这个文字是加粗的吗？</strong>

### 网页固定结构

<html>

	<head>
	<title>网页标题</title>
	</head>
​	<body>

​	网页主体

​	</body>

</html>

主要采用vs code开发

shift+1回车直接生成骨架

ctrl+/ 注释 ztrl+z撤回

### 单标签（不需要确定开始结束）例如：

1.<br>（换行）

2.<hr>

（水平线）

### 标题标签h标签

https://www.runoob.com/html/html-basic.html

<h1>这是标题 1</h1>
<h2>这是标题 2</h2>
<h3>这是标题 3</h3>
<h4>这是标题 4</h4>
<h5>这是标题 5</h5>
<h6>这是标题 6</h6>

默认加粗，占一行

### 段落标签<p>标签

<p>这是chengrui的一个段落</p>

<p>这是chengrui的另一个段落</p>

独占一行，自动换行

### 文本格式化标签

b 加粗                               strong

u下划线                              ins

i 倾斜                                   em

s 删除线                              del

### 媒体标签

<img src="" alt="" title="这是title文字，当鼠标悬停时显示">                                                                    

 alt替换文本                                                                                                                                                   

title提示文本

width/height调整图片宽高，只设置一个是按比例缩放

### 路径

绝对路径（了解）

目录下的绝对路径，可直接到达目标位置，通常从盘符开始

相对路径

