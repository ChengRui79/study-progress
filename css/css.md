# css

## day1

### 基础认知

css:层叠样式表

​    /* css注释 */

​    /* 选择器{css属性} */

​    /* 选择器：查找标签 */

引入方式：内嵌式，外联式，行内式

外联式：<link rel="stylesheet" href="./day1.css">

### 选择器

选择器{css属性} ，选中的标签都将统一属性，可采用类选择器

类选择器：.类名{css属性}

可引用多个类选择器（class中空格隔开即可）

id选择器：#id{css属性}

id选择器不能重复使用（唯一性，为了配合js）

通配符选择器：*{css属性}

找到页面所以标签设置样式，一半用于去除标签默认的margin与padding

### 字体和文本样式

font-size字体大小

font-weight字体粗细normal(400),bold(700)

font-style文字倾斜normal，italic（<em>em</em>标签默认倾斜）

font-family文字字体

font属性具有复合属性，可连写（font：style weight size family）