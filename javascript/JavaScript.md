# JavaScript

## day1

    <script>
    alert('这是我的javascript day1')
    </script>

是运行在客户端的脚本语言（不需要编译，运行时由js解释器进行逐行解释并执行）

JavaScript由BOM、DOM、ECMA组成

### 位置

行内

内嵌

外部

### 注释

//单行 ctrl+/

/*多行shift+alt+a

*/

### 输入输出语句

​    //prompt这是一个输入框

​    prompt('请输入您的年龄')

​    //alert弹出警示框

​    alert('您确定？')

​    //console控制台输出

​    console.log('我是程序员能看到的')

### 变量

一个装载数据的容器

初始化并赋值

  var myname  = prompt('请输入您的用户名')

  alert('您好'+myname)

更新变量

var age=18;

age=19;最后结果是19

声明多变量

var age=18,

name=cr,

gz=10000;

只声明不赋值结果返回undefined

不声明不赋值直接报错

不声明，赋值可以但变成全局变量

变量命名规则：

严格区分大小写；

不能数字开头；

不能是关键字或保留字；

变量名要有意义；

驼峰命名法；

交换变量（需要一个临时变量）

​    var temp;

​    var apple1='青苹果';

​    var apple2='红苹果';

​    temp=apple1;

​    apple1=apple2;

​    apple2=temp;

​    console.log(apple1)

​    console.log(apple2)

## day2

### 数据类型

js的变量数据类型是根据等号右边数据类型确定

js是动态语言 变量的数据类型是可以变换的

简单数据类型有：number（数字型，包括小数和整数，八进制，在数字前加0，十六进制，在数字前加0x，NaN表示非数字），boolean（true参与运算当1，flase参与运算当0），string（使用‘’/“”，涉及引号嵌套，外双内单或外单内双，\n换行，\\斜杠，\b空格，\t缩进），null，undefined（数据未赋值）

isNaN（）方法判断是否为非数字，是数字返回false，不是数字返回true

string使用+进行拼接，只要有字符串与其他类型数据拼接，最终结果一定是字符串

typeof检测数据属于什么类型

### 数据类型的转换

转换为字符串类型

​    //1.toString方法

​    var num=10;

​    var str=num.toString();

​    console.log(typeof str);

​    //2.String(变量)

​    console.log(String(num));

​    //3.+拼接字符串方法

​    console.log(num+'');

转换为数字类型

​    //1.parseInt()把字符型转换为数值型，得到的是整数(取整)

​    // var age1=prompt('请输入您的年龄：')

​    // console.log(parseInt(age1));

​    console.log(parseInt('3.14'));//3

​    console.log(parseInt('102px'));//102

​    //2.parseFloat(),把字符型转换为数值型，得到的是小数，浮点数

​    console.log(parseFloat('3.14'));//3.14

​    console.log(parseFloat('102px'));//102

​    //3.Number()

​    var str1='123';

​    console.log(Number(str1));

​    console.log(Number('123'));

​    //利用- * 、隐式转换

转换为布尔型

Boolean()只能将'',0,NaN,null,undefined转换为false，其他均为true

#### 加法器

​    var num2=prompt('请您输入第一个值');

​    var num3=prompt('请您输入第二个值');

​    var result=parseFloat(num2)+parseFloat(num3)

​    alert('您的结果是'+result)