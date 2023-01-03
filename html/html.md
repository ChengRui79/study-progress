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

#### 路径

绝对路径（了解）

目录下的绝对路径，可直接到达目标位置，通常从盘符开始

相对路径

从当前文件出发找目标文件

同级<img src="./index.jpg" alt="我是替换文本" title="这是title文字，当鼠标悬停时显示" width="1500">

下级<img src="images/index.jpg" alt="我是替换文本" title="这是title文字，当鼠标悬停时显示" width="1500">

 上级<img src="../images/index.jpg" alt="我是替换文本" title="这是title文字，当鼠标悬停时显示" width="1500">

#### 音频标签

<audio src="../images/music.mp3" controls loop autoplay></audio>

src图片路径

controls显示播放的控件

autoplay自动播放（部分浏览器不支持）

loop循环播放

支持MP3、wav、ogg

#### 视频标签

<video src="../images/video.mp4" controls muted loop></video>

src图片路径

controls显示播放的控件

autoplay自动播放（谷歌浏览器需配合muted实现静音播放）

loop循环播放

#### 超链接标签

<a href="../day1/day1.html">超链接</a>

网站开发初期，还不知道跳转网址时，href值填#

<a href="#">超链接</a>

target属性默认_self(覆盖当前页面)，可以使用_blank跳转新页面

<a href="../day1/day1.html" target="_blank">超链接</a>

## day2

### 列表标签

#### 自定义列表

<dl>

  <dt>帮助中心</dt>

  <dd>账户管理</dd>

  <dd>帮助中心</dd>

</dl>

dl表示自定义列表主体

dt表示列表的主题

dd表示针对主题的内容



#### 有序列表

<ol>

  <li>chengrui:100</li>

  <li>leafming:98</li>

  <li>chery:96</li>

</ol>

ol标签只能有li标签，li标签里面随便放

#### 无序列表

<ul>

  <li>榴莲</li>

  <li>香蕉</li>

  <li>苹果</li>

  <li>哈密瓜</li>

  <li>火龙果</li>

</ul>

ul标签只能有li标签，li标签里面随便放

### 表格标签

table表格整体包裹tr

tr代表行包裹td

td代表单元格包裹内容

#### 表格相关属性

border边框宽度

width表格宽度

height表格高度

<table border="1" width="500" heighr="300">
    <tr>
        <td>姓名</td>
        <td>成绩</td>
        <td>评语</td>
    </tr>
    <tr>
        <td>chengrui</td>
        <td>100</td>
        <td>good</td>
    </tr>
    <tr>
        <td>leafming</td>
        <td>95</td>
        <td>good</td>
    </tr>
    <tr>
        <td>Cheryl</td>
        <td>93</td>
        <td>good</td>
    </tr>
</table>

实际开发样式效果采用css实现

#### 表格标题及表头单元格标签

caption表格大标题

th表头单元格

<table border="1" width="500" heighr="300">
    <caption><strong>学生成绩单</strong></caption>
    <tr>
        <th>姓名</th>
        <th>成绩</th>
        <th>评语</th>
    </tr>
    <tr>
        <td>chengrui</td>
        <td>100</td>
        <td>good</td>
    </tr>
    <tr>
        <td>leafming</td>
        <td>95</td>
        <td>good</td>
    </tr>
    <tr>
        <td>Cheryl</td>
        <td>93</td>
        <td>good</td>
    </tr>
</table>

#### 表格的结构标签

thead表格头部

tbody表格主题

tfoot表格底部

<table border="1" width="500" heighr="300">
    <caption><strong>学生成绩单</strong></caption>
    <thead>
    <tr>
        <th>姓名</th>
        <th>成绩</th>
        <th>评语</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td>chengrui</td>
        <td>100</td>
        <td>good</td>
    </tr>
    <tr>
        <td>leafming</td>
        <td>95</td>
        <td>good</td>
    </tr>
    </tbody>
    <tfoot>
    <tr>
        <td>Cheryl</td>
        <td>93</td>
        <td>good</td>
    </tr>
    </tfoot>
</table>

#### 合并单元格

跨行用rowspan跨列用colspan

左上原则确定删谁给保留单元格加属性

<table border="1" width="500" heighr="300">
    <caption><strong>学生成绩单</strong></caption>
    <thead>
    <tr>
        <th>姓名</th>
        <th>成绩</th>
        <th>评语</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td>chengrui</td>
        <td rowspan="2">100</td>
        <td>good</td>
    </tr>
    <tr>
        <td>leafming</td>
        <!-- <td>100</td> -->
        <td>good</td>
    </tr>
    </tbody>
    <tfoot>
    <tr>
        <td>Cheryl</td>
        <td>93</td>
        <td>good</td>
    </tr>
    </tfoot>
</table>

不能跨tbody，thead，tfoot

### 表单标签

#### input系列标签

标签名input

type属性：text（文本框），password（密码框），radio（单选框），checkbox（复选框），file（文件选择），submit（提交按钮），reset（重置按钮），button（普通按钮）

password（密码框），radio（单选框）可使用placeholder属性（提示字）

用户名：<input type="text" placeholder="请输入用户名">

密码框：<input type="password" placeholder="请输入密码">

name属性对radio（单选框）有分组功能，checked属性可设置radio默认选中

性别：<input type="radio" name="sex" checked>男<input type="radio" name="sex">女

file（文件选择）multiple属性（多文件上传）

submit（提交按钮），reset（重置按钮），需要一个表单域标签form

#### button按钮标签

type属性：submit，reset，button

谷歌浏览器button默认为提交

#### 下拉菜单

select下拉菜单整体

option下拉菜单每一项（selected属性默认选中）

<select>

  <option>北京</option>

  <option>上海</option>

  <option selected>苏州</option>

  <option>南京</option>

</select>

#### textarea文本域

cols可见宽带

rows可见行数

通常用css定义其属性

#### label标签

性别：

法1<input type="radio" name="sex" checked id="nan"><label for="nan">男</label>

法2<label><input type="radio" name="sex">女</label>

#### 语义化标签

##### 无语义标签

div一行只显示一个（独占一行）

span一行显示多个

##### 有语义标签（手机端网页用）

<header>网页头部</header>

<nav>网页导航</nav>

<footer>网页底部</footer>

<aside>网页侧边栏</aside>

<section>网页区块</section>

<article>网页文章</article>

### 字符实体

空格：&nbsp;

版权:&copy;

元：&yen;

欧元：&euro;

镑：&pound;
