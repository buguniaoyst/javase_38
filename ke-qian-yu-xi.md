# 课前预习

---

## 1、day01学习目标

* Java概述、**helloworld案例**

* 工具安装 、配置环境变量、注释、关键字

* 常量、变量、数据类型、标识符

## 2、课程内容简介

### 2.1、计算机常识

#### 2.1.1、人机交互【了解】

人机交互其实是人、应用软件和操作系统还有硬件之间的交互过程。

人机交互有两种体现方式：图形化界面和命令行

* **图形化界面**

图形界面（简称GUI）是指采用图形方式显示的计算机操作用户界面。与早期计算机使用的命令行界面相比，图形界面对于用户来说在视觉上更易于接受。常见的图形化界面有：电脑桌面操作，平板，手机等。

* **命令行**

命令行方式\(Command Line Interface CLI\)：需要有一个控制台\(dos窗口\)，输入特定的指令，让计算机完成一些操作。Command是系统命令执行程序的意思。常见的命令行操作方式有：linux命令操作和windos中的dos命令操作。

##### 1、两种人机交互方式对比

图形化界面操作方式：简单直观，易于接受，容易上手，是目前最流行的人机交互方式；

命令行操作方式：比较麻烦，需要记住一些命令；

##### 2、命令行操作

###### 2.1、打开控制台（dos窗口）

* 第一种方式：右键Windows开始------》运行-----》在运行框中输入cmd------》点击确定按钮,打开即可。

* 第二种方式：Windows打开控制台的方式： windows键+R 会出现运行窗口，在窗口中输入cmd，就可以打开控制台（dos窗口）。

###### 2.2、输入特定的命令

在控制台中不能随意的输入命令，要输入的命令必须保证操作系统可以识别。只有输入的正确的命令，操作系统才会去完成我们的想要的结果。

下一小节，将着重介绍这些特定的命令。

#### 2.1.2、常用dos命令【了解】

dos命令很多，但是开发中常用的不是很多，以下列举的都是使用频率比较高的命令：

##### 1、help

它可以列出windows中的所有dos命令

##### 2、dir

是directory的缩写。表示 显示一个目录中的文件和子目录\(文件夹\)。

##### 3、cd

显示当前目录的名称或将其更改。

* 1\)进入e盘： e：

* 2\)显示当前目录的名称：cd

* 3\)进入e盘中的某个文件夹中需要使用cd change directory cd itcast 进入itcast目录中

* 4\)退回到上一级目录：cd .. 例如： e:/itcast/a 退出a目录 cd.. 退回到e:/itcast

* 5\)直接退到根目录：cd 。注意 / 这个叫做斜线， 这\个叫做反斜线。

##### 4、cls

cls命令：清除屏幕上的信息。

##### 5、exit

exit命令：退出dos窗口。

### 2.2、Java概述

#### 2.2.1、Java语言的发展史【了解】

JAVA是SUN\(Stanford University Network，斯坦福大学网络公司\)1995年推出的一门高级编程语言。创始人是James Gosling\(詹姆斯.高斯林\)被业界称为java之父。

1982年，Sun Microsystems公司诞生于美国斯坦福大学校园。Sun公司1986年上市，在NASDAQ\(纳斯达克,是全美证券商协会自动报价系统\)的标识为SUNW，2007年改为JAVA.

2009年4月20日 19 点 40 分 美国数据软件巨头甲骨文公司\(Oracle\)宣布以74亿美元收购Sun公司。

随着Java技术在web方面的不断成熟，JAVA已经成为Web应用程序的首选开发语言。

由于互联网不断兴起，而Java语言正好是面向互联网的程序语言，所以Java也越来越火，直到今天，依然很火。

简单易学，完全面向对象，安全可靠，与平台无关的编程语言。

#### 2.2.2、Java语言的三种架构【了解】

Java语言对于开发方向又提供了三种技术方式，也就是三种架构方向。不同的架构可以应用到不同的领域中。

* J2SE：标准版，可以开发普通桌面的应用程序，Java语言的标准，学习Java的基础。例如：feiq，扫雷，扑克牌等。

* J2EE:企业版，是企业级的开发，主要面向企业，针对web应用程序的开发。

* J2ME:小型版，主要用于开发电子消费产品。如手机中的应用程序，现在已经被安卓取代。

#### 2.2.3、Java语言跨平台原理【了解】

使用Java应用开发的软件可以在任何平台上运行。一次编写到处运行

* 1 什么是跨平台

平台：可以指多方面，如职业平台，那在我们这里指的是操作系统。

跨平台：Java编写的程序或者软件不仅可以在windows上面运行，还可以在Linux和mac上面运行，这就是可以在任何操作系统上面运行

* 2 跨平台原理

Java开发的所有程序都可以在任何的操作系统上运行，主要是因为在不同的操作系统上装上了不同的软件（Java虚拟机）。Jvm（Java Virtual Machine）

#### 2.2.4、Java开发环境搭建【掌握】

在搭建环境之前我们首先要了解两个概念：JRE和JDK。

* 1 JRE

  ```
  Jre的全英文名是：Java Runtime Environment   Java运行环境。
  ```

* 2 JDK

  ```
  Jdk(Java Development Kit):java开发工具包。

  jdk提供给Java开发人员使用的。我们使用jdk开发的程序要交给jre去运行。
  ```

* 3 JDK的下载

  ```
    官方网址：www.oracle.com 。去官网下载jdk。
  ```

* 4 JDK的安装与测试

安装：正常安装，注意安装目录中不要有中文或者空格。

测试：打开dos窗口进入JDK安装目录中的bin目录，输入java，javac命令，如果能正常显示jdk中的信息则说明安装成功。

### 2.3、书写HelloWorld

#### 2.3.1 编写程序

使用EditPlus创建你一个Hello.java文件，然后在这个文件中书写以下代码：

```java
public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

#### 2.3.2编译Hello.java文件

通过javac Hello.java将Hello.java文件编译成Hello.class文件。

#### 2.3.2 运行程序

通过命令java Hello命令直接运行Hello.class文件。

### 2.4、环境变量

* 1.为什么要配置？

  希望在任何的目录下都可以去运行我们安装的JDK中bin目录下的程序。

  程序的编译和执行需要使用到javac和java命令，所以只能在bin目录下写程序

  实际开发中，不可能把程序写到bin目录下，所以我们必须让javac和java命令在任意目录下能够访问。

* 2.怎么配置？

  1、创建新的变量名称：JAVA\_HOME

  计算机-右键属性-高级系统设置-高级-环境变量-系统变量

  2、为JAVA\_HOME添加变量值：JDK安装目录 即 E:\Java\jdk1.7.0\_51  
  （这个路径以你自己的jdk安装目录为准）

  3、在path环境变量最前面添加如下内容：

  %JAVA\_HOME%\bin;

### 2.5、Java中的关键字，标识符，符号和注释

#### 2.5.1 关键字

HelloWorld里面写的东西，比如说蓝字部分，class ，public，static。这些都属于关键字。不同的关键字，在Java代码中有不同的使用场景。

关键字：在Java语言中被赋予了特定含义的一些单词或者字母的组合。

如**class**：它在Java中是用来定义（创建）Java中的一个程序的开始。

#### 2.5.2 标识符

标识符：表示起一定标识作用的符号。标识作用的符号指的是在程序中定义的名称。比如Demo，haha等。

main也是标识符，他是方法的名称。

方法或者类的名字可以让我们找到我们想使用的方法或者类使用。

标识符定义名字不能随便起，标识符定义是有规范的，只要不破坏这个规范，就没事，破坏就非法。

##### 2.5.2.1    标识符的组成

* 1、标识符由a-z ，26个英文字母大小写。同时还有0-9这十个数字，同时还有 \_\(下划线\)  $（美元符） 。标识符只能由这些符号组成。

##### 2.5.2.2    标识符的书写规定

* 1、不能以数字开头；

* 2、不可以使用关键字，因为关键字已经被特殊定义了；

#### 2.5.3    符号

书写的Java代码中常用的符号：

{} ：它一般是在划定程序某些代码区域（范围）。

\(\) ：它表示的左侧一般是一个方法名，一般用在方法上。

英文分号：在java中一句话写完，一般需要一个分号结束。

\[\] ：它表示的内容是数组。

#### 2.5.4    注释

##### 1    注释介绍

注释：对Java中的程序代码进行解释说明的文字。

那么这里有了说明以后我们就要把不是代码的说明注释起来，不要让编译器对他操作了，引发编译错误。

Java语言中的注释有三种格式：

* 1）单行注释：单行注释的表现很简单，只要在开头写两个斜杠就可以了。

用法：//后面书写注释的内容

注意：单行注释里面可以写单行注释

* 2）多行注释：有开始就得有结束。/\*\*/

用法：

/\*

注释的内容

\*/

注意：单行和多行注释，很多的语言都是支持的。而接下来讲的第三种注释只有Java语言支持，这个是Java特有的注释。

多行注释不能有多行注释。

* 3）文档注释：文档注释稍微特殊，在文档注释里面可以写程序的作者，程序的版本等。同时在文档注释里面也可以写点注释的文字信息。

用法：

/\*\*

@author 作者

@version 版本

注释的内容

\*/

说明：前面加个@符号，说明这个单词是可以被解析的。

注意：

1、单行和多行注释，很多的语言都是支持的。而第三种注释文档注释只有Java语言支持，这个是Java特有的注释。

2、注释的内容仅仅是对源代码进行解释说明，而使用javac 编译之后生成的class文件中是不会存在的。

3、要求后期大家在写Java代码的时候，源代码中都需要添加注释。

注释的作用：

1）对程序进行说明

2）调试程序

【代码示例】

```java
/*
    注释：用于解释说明程序的文字

    分类：
        单行
        多行

    作用：解释说明程序，提高程序的阅读性
*/

//这是我的HelloWorld案例
class HelloWorld {
    /*
        这是main方法
        main是程序的入口方法
        所有代码的执行都是从main方法开始的
    */
    public static void main(String[] args) {
        //这是输出语句
        System.out.println("HelloWorld");
    }
}
```

### 2.6 语法格式

#### 2.6.1常量

在我们的生活中会有一些固定不变的数据，而Java语言又是解决生活中问题的，那么Java就必须把生活中这些固定不变的数据也要进行相应的描述。

在Java中要描述一些固定不变的数据，这时就需要使用Java中的常量这个概念来描述。

##### 1    常量概述

常量：不能被改变的数据，固定不变的数据。

##### 2    常量分类

* 1）数值型：

  生活中的数字：1,2,8,18等

  整数：1,2,3等

  小数：1.1,1.2,2.3等

* 2）字符型：生活中的单个数字 汉字 字母 符号 等，

  Java中单个数据，字符，Java中的字符书写需要使用英文单引号（‘’）引用。并且单引号中有且只有一个字符数据。

  ‘你’   ‘A’

  这不是字符：’abc’

  ‘+’ ‘-’等是字符

  注意：字符表示单引号里面只有一个字母、数字或者符号。所以’123’不表示字符。

* 3\) 字符串型：生活中的一句话

  Java中的字符串需要使用英文双引号（“”）引用。在Java中使用双引号把多个字符串在一起， 我们就称为字符串。

  “abc”   “hello world”  “a”  “” 表示空字符串

* 4）布尔型（boolean）：生活中的判断后的真假 对错

  Java中需要使用 true ：真 或 false：假 表示。

* 5）空常量型：只有一个数值就是null，给引用数据类型赋值的，后面会讲解。\(了解\)

#### 2.6.2    变量

##### 1    变量概述

变量的官方定义：它表示的是一个空间，在程序运行的过程中，可以随时去更改这个空间中的数据。体现在计算机中，就表示的是计算机内存中的一个存储区域。

常量：表示不能被改变的数据。就是一个固定的量\(值\)，不能改变。

变量：就是一个可以改变的量\(值\)，可以改变其值。

在Java程序中，需要保存数据，这时首先需要在内存中开辟一个空间，然后把数据保存在这个空间中。

##### 2    变量定义格式

变量有两种书写格式：

* 1）空间中保存的数据类型  空间名称  ; ------&gt;数据类型 变量名;

举例：整数 x;

* 2\) 空间中保存的数据类型  空间名称  =  空间中要保存的数据;

------&gt;数据类型 变量名=初始值（常量值）;

举例：整数 x= 6;

##### 3    变量的起名

空间名称就是变量名称。它就是一个普通的标识符。

书写规范：

如果变量名是由多个单词组成，第一个单词全部小写，从第二个单词开始，首字母大写。

##### 4    变量的注意事项

* 1、变量空间在使用之前需要先保存初始化的数据。

* 2、Java中定义的变量，都有自己存在的范围。

#### 2.6.3    数据类型

##### 1    计算机存储单元

变量是内存中的小容器，用来存储数据。那么计算机内存是怎么存储数据的呢？无论是内存还是硬盘，计算机中最小的存储单位叫“字节（byte）”，字节是由连续的8个比特位\(bit\)组成。

除了字节外还有一些常用的存储单位，大家可能比较熟悉，我们一起来看看：

1个字节 = 8 个二进制数位。

1byte = 8bit  比特位

1kb =1024 byte

1 mb = 1024 kb

1gb= 1024 mb

1tb = 1024 gb

##### 2    数据类型概述和分类

Java中把数据共计划分成2大类型：

1）引用数据类型：它表示是数组  、 类 、接口等

2）基本数据类型：

对基本的数据进行的类型划分：

整数：由于整数有非常大的数据，也有非常小的数据。于是把整数类型又区分成4种：

byte 、 short 、 int 、 long

4个类型的区别：

byte 开辟的空间 占内存 1个字节。 范围 -128~127

short开辟的空间 占内存 2个字节。

int  开辟的空间 占内存 4个字节。

long 开辟的空间 占内存 8个字节。long l=12345678903L;

小数：

float\(单精度\)、double\(双精度\)

float 开辟的空间是 4 个字节

double 开辟的空间是 8 个字节

字符：

char     char占两个字节。

布尔：

boolean  true 真  false 假

boolean占一个字节。

这八种基本类型数据，就是前面介绍过的关键字。

数据类型具体划分如下图所示：

#### 2.6.4    定义变量

##### 1    基本数据类型变量的定义和使用

变量的定义格式：

```
    数据类型 变量名 = 初始化值;

基本数据类型：

    byte,short,int,long,float,double,char,boolean

注意：

    整数默认是int类型，定义long类型的数据时，要在数据后面加L。

    浮点数默认是double类型，定义float类型的数据时，要在数据后面加F。
```

6.4.2    案例代码

```java
public class VariableDemo {
    public static void main(String[] args) {
        //定义byte类型的变量
        byte b = 10;
        System.out.println(b);

        //定义short类型的变量
        short s = 100;
        System.out.println(s);

        //定义int类型的变量
        int i = 10000;
        System.out.println(i);

        //定义long类型的变量
        long l = 1000000000000000L;
        System.out.println(l);

        //定义float类型的变量
        float f = 12.34F;
        System.out.println(f);

        //定义double类型的变量
        double d = 12.34;
        System.out.println(d);

        //定义char类型的变量
        char c = 'a';
        System.out.println(c);

        //定义boolean类型的变量
        boolean bb = false;
        System.out.println(bb);
    }
}
```

注意：

1）在java中随便书写一个整数，默认是int类型，比如：12,13都是int类型；

2）在java中随便书写一个小数，默认是double类型，比如：3.14就是double类型；

#### 2.6.5    数据类型转换\(掌握\)

在java中，不同的数据需要保存在不同的空间中，而开辟空间的时候，需要通过不同的类型关键字来定义当前这个空间是什么类型的空间。

开辟的空间如果和保存的数据类型不一致，那么就很容易导致程序出现错误。

这时我们就需要使用数据类型的转换技术，完成数据的保存工作。

数据类型的转换，可以分为两种：

1）隐式类型转换（自动类型转换）自动类型提升

2）强制类型转换

##### 1    隐式数据类型转换

隐式类型转换：在程序中，空间保存的数据类型不一致的时候，java内部会自动的帮助我们转换。

要能够自动转换，必须遵守Java中的自动转换的规则：

可以把小空间中的数据给大空间中保存。

byte 空间中的数据， 可以自动的转成 short int long float double

但是不能把double 保存在 byte 、int 、 short 、long 等空间。

##### 2    案例代码

```java
/*
    +:是一个运算符，做加法运算的。
    我们在做运算的时候，一般要求参与运算的数据类型必须一致。

    类型转换：
        隐式转换
        强制转换

    隐式转换    
        byte,short,char -- int -- long -- float -- double
*/
public class TypeCastDemo {
    public static void main(String[] args) {
        //定义两个int类型的变量
        int a = 3;
        int b = 4;
        int c = a + b;
        System.out.println(c);

        //定义一个byte类型,定义一个int类型
        byte bb = 2;
        int cc = 5;
        System.out.println(bb + cc);

        //我能不能不直接输出，用一个变量接收呢?
        //用变量接收，这个变量应该有类型
        //可能损失精度
        //byte dd = bb + cc;
        int dd = bb + cc;
        System.out.println(dd);
    }
```

转换规律：

容量小的类型可自动转换为容量大的数据类型；

##### 3    强制类型数据转换

注意：

强制类型转换：它一般都会有数据的丢失。不建议强制转换。

格式：

需要转成的数据类型 变量名 = \( 需要转成的数据类型 \)\( 被转的数据 \);

##### 4    案例代码

int i4 = \(int \)dd + 3.14; 报错。------》int i=\(int\)\(dd+3.14\);编译成功。

