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
var temp；  
var apple1='青苹果';  
var apple2='红苹果';  
temp=apple1;  
apple1=apple2;  
apple2=temp;  
console.log(apple1)  
console.log(apple2)  
