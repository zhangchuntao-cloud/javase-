# javase

## 快捷键:

* ctrl+p显示参数列表
* ctrl+alt+v自动生成左边
* ctrl+alt+t选择语句包围
* alt+回车:将左右进行切割, 转换多态类型
* ctrl+b:查看源码
* shift+f6批量修改
* ctrl+shift+u:变成大写upper
* 查看源码:ctrl+n搜索LinkedList选择所有位置alt+7显示大纲视图



## 一.环境变量和java运行了解

### 1.1人机交互和cmd:

* 人机交互:
	* 施乐公司1981年推出施乐之星，图形化界面雏形，引入窗口模式, 图形化界面的缺点–>消耗内存&&运行速度慢


* cmd描述:

	* windows中利用命令行的方式操作计算机

	* 常见的CMD命令

		* 盘符名称+冒号(不加cd)
			* 盘符切换 E：回车
		* dir
			- 查看当前路径下的内容（包括隐藏的）
		
		- cd目录1\目录2\\…
			- （tab可以自动补充）
		- cd \
			- 退回根目录
		- exit
			- 退出当前指令
		- cls
			- 清空


### 1.2环境变量配置

​	操作步骤：

1. windows+E此电脑右键属性--高级系统设置–环境变量–path编辑–QQ的位置copy进去，然后就可以再path之中打开QQ.exe了(简单的)。

2. path环境变量配制(变成哪里都能用这四个exe)

	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016185254567.png" alt="image-20251016185254567" style="zoom: 25%;" />

​			

​			

### 1.3了解java发展安装和运行:

* 学习方法：先从广度；

####  1.3.1安装ide:

![image-20251016155732425](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016155732425.png)

​		01:	bin:存放了各种工具和命令（javac和java）

​		02:	conf:相关配置文件

​		03： include： 平台特定头文件

​		04： jmods:	各种模块

​		05： legal:	各模块的授权文档

​		06： lib:	工具的一些补充jAR包



<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016160459497.png" alt="image-20251016160459497" style="zoom:25%;" />

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016160423082.png" alt="image-20251016160423082" style="zoom:25%;" />

* 文件扩展名就是后缀

	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016162950458.png" alt="image-20251016162950458" style="zoom: 25%;" />

* 可能的bug:符号要在英文状态下

* 发展:James Gosling”java之父”

#### 1.3.2java分类和运行:



* java的分类:
	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016200928704.png" alt="image-20251016200928704" style="zoom:25%;" />

	* javaSE: 桌面应用


	* javaME:移动开发/嵌入式开发


	* javaEE:服务器开发

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251031215356315.png" alt="image-20251031215356315" style="zoom:25%;" />
* java的运行:
* java跨平台原理

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016203140239.png" alt="image-20251016203140239" style="zoom:25%;" />



​			JVM:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016203325639.png" alt="image-20251016203325639" style="zoom: 33%;" />

​			JDK:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016203649786.png" alt="image-20251016203649786" style="zoom:25%;" />

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016204046270.png" alt="image-20251016204046270" style="zoom:25%;" />

 			JDK包含了JRE(java的运行环境)

## 二.java的基本概念

### 2.1代码了解

* 注释:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016205055141.png" alt="image-20251016205055141" style="zoom:25%;" />

* 关键字:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016205621203.png" alt="image-20251016205621203" style="zoom: 50%;" />

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016205708028.png" alt="image-20251016205708028" style="zoom: 50%;" />

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016205728936.png" alt="image-20251016205728936" style="zoom: 50%;" />

​	①:class:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016210657035.png" alt="image-20251016210657035" style="zoom: 50%;" />

* 字面量类型:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016210817280.png" alt="image-20251016210817280" style="zoom:33%;" />

[^举例]:比如‘abc’啥也不是(单括号),null不能打印

* 制表符 \t

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251016213135564.png" alt="image-20251016213135564" style="zoom: 50%;" />

### 2.2数据进制和数据类型

* 数据进制

	* 不同进制在代码中的表现形式:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017131114952.png" alt="image-20251017131114952" style="zoom:50%;" />


	* 转换:
		* 电脑里面的计算器程序员模式
		* 辗转相除法取每次余数


* .计算机的存储规则

  * 计算机中,任何数据都是以二进制的形式存储

  * 二进制中一个0或一个1叫做一个bit(比特位). 把8个bit作为一组, 那么就可以存储2^8(256)个数据, 叫做一个字节, 是计算机当中最小的存储单元

  * ![image-20251107165716900](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251107165716900.png)

  * <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017133317398.png" alt="image-20251017133317398" style="zoom:50%;" />
  * windows系统默认使用的就是GBK![image-20251107170235947](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251107170235947.png)

* 三原色:红绿蓝(初代御三家)
  * <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017142902907.png" alt="image-20251017142902907" style="zoom:33%;" /><img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017143142780.png" alt="image-20251017143142780" style="zoom: 50%;" />

* 数据类型

  * ![image-20251017143747482](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017143747482.png)

  * 注意: long类型后缀加L(大小写都可以);
  	          float类型后缀加F

* 标识符:就是给类,方法,变量等起的名字

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017150818360.png" alt="image-20251017150818360" style="zoom:67%;" />

* 命名规则:小驼峰,大驼峰

	键盘录入:

* 两套体系

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017154500429.png" alt="image-20251017154500429" style="zoom: 50%;" />



* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017160907425.png" alt="image-20251017160907425" style="zoom: 50%;" />

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017165819121.png" alt="image-20251017165819121" style="zoom:33%;" /><img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017165847817.png" alt="image-20251017165847817" style="zoom:50%;" />

## 三.java运算符

### 3.1数据类型转换

1.隐式转换:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017204416879.png" alt="image-20251017204416879" style="zoom:33%;" />

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017204602483.png" alt="image-20251017204602483" style="zoom:25%;" />

![image-20251017204859592](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017204859592.png)

2.强制转换:
<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017205707815.png" alt="image-20251017205707815" style="zoom: 50%;" />

3.数字字符形式转数字(或者-‘0’):
<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251022153409779.png" alt="image-20251022153409779" style="zoom:25%;" />

### 3.2算术运算符“+”

1.字符串的“+”操作

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017211956599.png" alt="image-20251017211956599" style="zoom: 33%;" />

2.字符的“+”操作

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017212705790.png" alt="image-20251017212705790" style="zoom: 25%;" />

辨析:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017213217493.png" alt="image-20251017213217493" style="zoom:67%;" />

​											②做的是字符串的拼接操作

3.自增自减运算符:
a++(先用后加);++a(先加后用);a–;–a

4.赋值运算符

a +=b(将a+b赋值给变量a,而且隐藏强制转换)

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251017214509347.png" alt="image-20251017214509347" style="zoom:33%;" />

5.关系运算符(==  !=  >  <  <=  >=)

* 结果是boolean类型

* ==号:
	* 对引用数据类型比的是地址值
	* 对基本数据类型比的是实际值

6.逻辑运算符(&  |  ^异或  !取反)

区分&&和&:

 <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018092109125.png" alt="image-20251018092109125" style="zoom: 50%;" />





<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018092232080.png" alt="image-20251018092232080" style="zoom: 50%;" /><img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018092324000.png" alt="image-20251018092324000" style="zoom:33%;" />

7.三元运算符:
![image-20251018092940304](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018092940304.png)

*(结果必须要被使用)*

8.运算符的优先级:()优先于所有.

### 3.3原码,反码,补码

①:原码:
![image-20251018105434917](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018105434917.png)

②:反码:

![image-20251018105515714](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018105515714.png)

* 弊端是跨0跟实际结果有1偏差的问题

③:补码:

* 目的:是为了解决负数计算时跨0问题
* 计算机中的存储和计算都是以补码的形式进行的

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018105652717.png" alt="image-20251018105652717" style="zoom:33%;" />

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018105720277.png" alt="image-20251018105720277" style="zoom:33%;" />

④:其他运算符:
<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018111308863.png" alt="image-20251018111308863" style="zoom:33%;" />

* &运算示例:

	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018111403385.png" alt="image-20251018111403385" style="zoom: 50%;" />

* |运算示例:
	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018111440860.png" alt="image-20251018111440860" style="zoom: 33%;" />

* 左移<<:
	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018111552323.png" alt="image-20251018111552323" style="zoom: 33%;" />

* 右移:
	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018111654884.png" alt="image-20251018111654884" style="zoom: 33%;" />

## 四.判断和循环

### 4.1.判断

* if:

![image-20251018113839450](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018113839450.png)

* switch:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018130503446.png" alt="image-20251018130503446" style="zoom:50%;" />

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018165501220.png" alt="image-20251018165501220" style="zoom: 50%;" />

* 新特性: 不用break的情况(只有一行时花括号可以省略)    <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018165646042.png" alt="image-20251018165646042" style="zoom:50%;" />

* 穿透性: <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018170728937.png" alt="image-20251018170728937" style="zoom:50%;" />

### 4.2循环

1.for循环新写法:
<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018172310615.png" alt="image-20251018172310615" style="zoom: 25%;" />

2.<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018172344285.png" alt="image-20251018172344285" style="zoom:50%;" />

3.循环高级:
①无限循环:
如for<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018191959374.png" alt="image-20251018191959374" style="zoom:33%;" />

* 随机数

```java
//1.导包
import java.util.Random;

public class random_numbers {
    public static void main(String[] args) {

        //2.创建对象
        Random r = new Random();

        //3.生成随机数
        //口诀:包头不包尾,包左不包右
        int number = r.nextInt(100);//0~99
        System.out.println(number);
    }
}
```

## 五.数组

### 5.1初始化和遍历

* 定义: 是一种存储同种类型的多个值的容器

* 静态初始化:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018213215190.png" alt="image-20251018213215190" style="zoom: 25%;" />

* 动态初始化:

* ```java
	public class arr {
	    public static void main(String[] args) {
	        //动态创建数组
	        //数据类型[] 数组名 = new 数据类型[数组长度];
	        String[] arr = new String[6];
	        //创建的时候,由我们自己指定数组长度,由虚拟机给出默认的初始值
	        //默认值:
	        //引用数据类型(String, 数组, 自定义类?):null
	        //整数数据类型:0
	        //布尔数据类型:false
	        //字符数据类型:'\u0000'
	        //小数类型:0.0
	        System.out.println(arr[0]);
	    }
	}
	```

* 地址:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251018213625168.png" alt="image-20251018213625168" style="zoom:33%;" />

* 注意点:一个循环尽量只做一件事

* 练习:

	* 求最值


	* 将数组逆序


~~~java
* 生成随机数组

	```java
	import java.util.Random;
	
	//将已知数组打乱顺序
	public class arr {
	    public static void main(String[] args) {
	        int[] arr = new int[]{1, 2, 3, 4, 5};
	        //生成随机索引,再交换
	        for (int i = 0; i < arr.length; i++) {
	            Random rand = new Random();
	            int randomIndex = rand.nextInt(arr.length);
	            //交换
	            int temp = arr[i];
	            arr[i] = arr[randomIndex];
	            arr[randomIndex] = temp;
	        }
	        //打印数组
	        for (int i = 0; i < arr.length; i++) {
	            System.out.println(arr[i]);
	        }
	    }
	}
~~~

### 5.2.数组的内存图:

1.java内存分配:
<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251019111748942.png" alt="image-20251019111748942" style="zoom: 25%;" /><img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251019111940718.png" alt="image-20251019111940718" style="zoom: 33%;" />

* 栈
	方法运行时使用的内存，比如main方法运行，进入方法栈中执行。(开始执行进栈,执行结束出栈)

* 堆
	存储对象或者数组，new来创建的，都存储在堆内存。

* 方法区
	存储可以运行的class文件。

* 本地方法栈
	JVM在使用操作系统功能时使用，和我们开发无关。

* 寄存器
	给CPU使用，和我们开发无关。

* *从JDK8开始, 取消方法区,新增元空间,原来方法区有的功能放到堆中,有的放到栈中*

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251019112324948.png" alt="image-20251019112324948" style="zoom:33%;" />

eg.(0x?)

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251019113245952.png" alt="image-20251019113245952" style="zoom:53%;" />

### 5.3.二维数组:

1.静态初始化:
<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020163517047.png" alt="image-20251020163517047" style="zoom:33%;" />

2.打印细节

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020163906395.png" alt="image-20251020163906395" style="zoom:33%;" />

3.内存分配:
<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020165422753.png" alt="image-20251020165422753" style="zoom: 25%;" />



4.特殊情况(添加两个长度不同的一维数组):

* 特殊情况1:
	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020165536552.png" alt="image-20251020165536552" style="zoom: 50%;" />

* 特殊情况2:
	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020165709347.png" alt="image-20251020165709347" style="zoom: 50%;" />

### 5.4可变参数:

```java
package Test;

public class test {
    public static void main(String[] args) {
        int sum = getSum(1,2,3,4);
        System.out.println(sum);//2+3+4=9
        //可变参数的小细节:
        //1.可变参数可以和普通参数一起放在形参列表中,但是必须保证可变参数在最后
        //2.一个形参列表中只能出现一个可变参数
    }
    public static int getSum(int a,int...args){
        int sum = 0;
        for (int i : args) {
            sum = sum + i;
        }
        return sum;
    }
}
```

```java
//创建集合添加元素的方法简化代码
private static <T> List<T> createList(T... elements) {
    List<T> list = new ArrayList<>();
    Collections.addAll(list, elements);
    return list;
}
```

## 六.方法:

### 6.1方法概述

* 程序中最小的执行单元.

* 提高代码的复用性;
* 提高代码的可维护性

### 6.2方法的重载:

* return:
	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251019142403101.png" alt="image-20251019142403101" style="zoom:33%;" />

* 定义:

![image-20251019142821959](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251019142821959.png)

* 判断是否构成重载:

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251019143150888.png" alt="image-20251019143150888" style="zoom: 50%;" />

不看返回值

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251019143316619.png" alt="image-20251019143316619" style="zoom: 67%;" />

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251019143400164.png" alt="image-20251019143400164" style="zoom: 50%;" />

不在一个类,不构成重载

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251019143500307.png" alt="image-20251019143500307" style="zoom: 50%;" />

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251019143558052.png" alt="image-20251019143558052" style="zoom: 50%;" />

虽然构成,但基本不会使用

### 6.3.基本数据类型和引用数据类型:

#### 1.基本数据类型:

* 定义:*变量中存储的是真实的数据*
* 数据值是存储在自己的空间中
* eg<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251019161532347.png" alt="image-20251019161532347" style="zoom:33%;" />



#### 2.引用数据类型:

* 定义:*变量中存储的是地址值, 其中引用是指使用了其他 空间中的数据.*
* 数据值存储在其他空间中,自己空间中存储的是地址值
* 特点:赋值给其他变量,赋的是地址值

* eg<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251019161639098.png" alt="image-20251019161639098" style="zoom:33%;" /><img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251019162018807.png" alt="image-20251019162018807" style="zoom: 25%;" />

## 七.面向对象:

### 7.1设计对象和使用:

* 理解面向对象:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020170907279.png" alt="image-20251020170907279" style="zoom:33%;" />

eg. 调用Scanner输入;Random生成随机数

* 类和对象:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020190549012.png" alt="image-20251020190549012" style="zoom: 33%;" /><img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020191249228.png" alt="image-20251020191249228" style="zoom:25%;" />

* 注意事项:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020191349538.png" alt="image-20251020191349538" style="zoom:33%;" />

1. 多个java文件在一个软件包中

* 建议一个文件定义一个class类

* 对象的成员变量默认值:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020191657276.png" alt="image-20251020191657276" style="zoom:33%;" />

### 7.2封装:

* 简单理解:
	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020195101355.png" alt="image-20251020195101355" style="zoom:30%;" />

* 工具:
	sun公司设计的各种对象,方法的java文档:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020195510414.png" alt="image-20251020195510414" style="zoom:33%;" />

#### 7.2.1关键字和构造方法:

* private

	* *是一个权限修饰符*

	* *可以修饰成员(成员变量和成员方法)*

	* *被private修饰的成员只能在本类中才能访问*


<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020200812009.png" alt="image-20251020200812009" style="zoom: 25%;" />

* > this:调用的是本类的成员变量
	
	* 区分成员变量和局部变量, 本质是代表方法调用者的地址值

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020214552756.png" alt="image-20251020214552756" style="zoom:25%;" />		

* 局部变量:方法中的变量;  成员变量:类中方法外的变量

* 构造方法:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020205037980.png" alt="image-20251020205037980" style="zoom:25%;" /><img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020205121263.png" alt="image-20251020205121263" style="zoom:25%;" />

#### 7.2.2三种情况的对象内存图:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020212729485.png" alt="image-20251020212729485" style="zoom:50%;" />

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020213444981.png" alt="image-20251020213444981" style="zoom: 25%;" />

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251020214059441.png" alt="image-20251020214059441" style="zoom:25%;" />











## 八.字符串:

### 8.1.API:

* 定义:目前JDK中提供的各种功能的java类

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251021202128532.png" alt="image-20251021202128532" style="zoom:25%;" />

#### 常用api:

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251026184626150.png" alt="image-20251026184626150" style="zoom:25%;" />

* math


##### 8.11system和arraycopy和Runtime:

* system是一个工具类, 提供了一些与系统相关的方法

* 统计时间

* 

* ```java
	public class test {
	    public static void main(String[] args) {
	        long start = System.currentTimeMillis();
	        //遍历1-10000中的质数
	        for (int i = 2; i <= 10000; i++) {
	            if(judge(i)){
	                System.out.println(i);
	            }
	        }
	        long end = System.currentTimeMillis();
	        System.out.println(end-start);
	        System.exit(0);
	    }
	    public static boolean judge(int number){
	        for (int j = 2; j <= Math.sqrt(number); j++) {
	            if(number%j==0){
	                return false;
	            }
	        }
	        return true;
	    }
	}
	```

* arraycopy:

* ```java
	public class test {
	    public static void main(String[] args) {
	
	        Student stu1 = new Student(23, "zhangsan");
	        Student stu2 = new Student(24, "lisi");
	        Student stu3 = new Student(25, "wangwu");
	        Student[] arr1 = {stu1, stu2, stu3};
	        Person[] arr2 = new Person[3];
	        
	        //子类可以拷贝给父类,在强制转换输出
	        System.arraycopy(arr1, 0, arr2, 0, 3);
	
	        for (int i = 0; i < 3; i++) {
	            Student s = (Student) arr2[i];
	            System.out.println(s.getName()+", "+s.getAge());
	        }
	    }
	}
	class Person{
	    private int age;
	    private String name;
	    public Person(){}
	    public Person(int age,String name){
	        this.age=age;
	        this.name=name;
	    }
	    public int getAge() {
	        return age;
	    }
	    public void setAge(int age) {
	        this.age = age;
	    }
	    public String getName() {
	        return name;
	    }
	    public void setName(String name) {
	        this.name = name;
	    }
	
	}
	
	class Student extends Person{
	    public Student(int age,String name){
	        super(age,name);
	    }
	    public Student(){
	        super();
	    }
	}
	```

* Runtime:

* ```java
  package test;
  
  import java.io.IOException;
  
  public class test{
      public static void main(String[] args) throws IOException {
          //1.获取Runtime的对象
          Runtime r1 = Runtime.getRuntime();
  
          //2.exit 停止虚拟机
          //Runtime.getRuntime().exit(0);
          //3.获得CPU的线程数
          System.out.println(Runtime.getRuntime().availableProcessors());
          //4.总内存大小,单位:byte字节
          System.out.println(Runtime.getRuntime().maxMemory());
          //5.已获取的总内存大小, 单位:byte字节
          System.out.println(Runtime.getRuntime().totalMemory()/1024/1024);
          //6.剩余内存大小
          System.out.println(Runtime.getRuntime().freeMemory()/1024/1024);
          //7.运行cmd命令
          Runtime.getRuntime().exec("shutdown -a");
      }
  }
  ```

##### 8.12object和clone(深浅)和objects:

* object:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251026155629272.png" alt="image-20251026155629272" style="zoom:25%;" />

* clone(深浅)

* (默认浅克隆, 如果需要深克隆需要重写方法或者使用第三方工具类):

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251027095224777.png" alt="image-20251027095224777" style="zoom:25%;" />
* 浅拷贝:直接拷贝变量的地址值<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251027091610235.png" alt="image-20251027091610235" style="zoom: 67%;" />* 
* 深克隆:如果是基本数据类型,跟原来一样,把变量记录的数据值直接拷贝过来;  如果是引用数据类型, 不会拷贝地址值,而是在外面重新创建一个对象<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251027092222579.png" alt="image-20251027092222579" style="zoom:40%;" />
	* 解释:String是引用数据类型,但是特点是只要不是手动new的, 都是会在串池当中进行管理的,字符串会复用

* Objects:

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251027142248856.png" alt="image-20251027142248856" style="zoom:25%;" />

##### 8.13BigInteger和BigDemical:

* BigInteger:
	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251027160444894.png" alt="image-20251027160444894" style="zoom:40%;" />



* ```java
	public class Test {
	    public static void main(String[] args) {
	        //1.获取一个随机的大整数, public BigInteger(int num, Random rnd) 获取随机大整数, 范围:[0~2的num次方-1]
	        Random r = new Random();
	        BigInteger bi1 = new BigInteger(4, r);//[0~15]
	        System.out.println(bi1);
	
	        //2.public BigInteger(String val)  获取指定的大整数
	        BigInteger bi2 = new BigInteger("9999999999999999");//9999999999999999
	        System.out.println(bi2);
	        //"1.2", "abc"会报错
	
	        //3.获取指定进制的大整数  public BigInteger(String val, int radix)
	        BigInteger bi3 = new BigInteger("100", 2);//转换为2进制
	        System.out.println(bi3);
	        
	    }
	}
	```

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251027151608727.png" alt="image-20251027151608727" style="zoom:33%;" />

	* 对17的解释:BigInteger是引用数据类型

* ![image-20251027152802631](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251027152802631.png)

* 查看原码得到的, 对比一下:

* ```java
	public class Test {
	    public static void main(String[] args) {
	        StringBuilder a = new StringBuilder("a");
	        StringBuilder b = new StringBuilder("b");
	        //添加
	        StringBuilder result = a.append(b);
	        System.out.println(result);//ab
	        System.out.println(a==result);//true
	    }
	}
	```


* BigDecimal:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251027170108286.png" alt="image-20251027170108286" style="zoom:25%;" /><img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251027164551170.png" alt="image-20251027164551170" style="zoom: 25%;" />

##### 8.14正则表达式


* 正则表达式:api帮助文档里搜pattern<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251027185030332.png" alt="image-20251027185030332" style="zoom:25%;" />

  * 常见的一些:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251027203309086.png" alt="image-20251027203309086" style="zoom:25%;" />

  * <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251027203330624.png" alt="image-20251027203330624" style="zoom:25%;" />

  * 爬取

  * ```java
  	public class test {
  	    public static void main(String[] args) {
  	        String str = "Java是一门高级、面向对象、跨平台的编程语言。它的核心设计理念是 “一次编写，到处运行”,有Java11和Java17等版本";
  	        //1.获取正则表达式的对象
  	        Pattern p = Pattern.compile("Java\\d{0,2}");
  	        //2.获取文本匹配器的对象
  	        //拿着m去读str
  	        Matcher m = p.matcher(str);
  	        while (m.find()) {
  	            System.out.println(m.group());
  	        }
  	    }
  	}
  	```

  * 捕获分组和非捕获分组<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251027214843098.png" alt="image-20251027214843098" style="zoom:25%;" />

  * ```java
  	package Test;
  	
  	public class test {
  	    public static void main(String[] args) {
  	       String str = "我要要要要学学学编编程程程程";
  	       //\\1表示再一次出现, $1表示把正则表达式中第一组的内容再拿来用
  	        //正则内部:\\组号   外部:$组号
  	       String result = str.replaceAll("(.)\\1+", "$1");
  	        System.out.println(result);
  	    }
  	}
  	```

##### 8.15时间类和包装类:

* 时间类:

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251027215521867.png" alt="image-20251027215521867" style="zoom: 50%;" />

* Date时间类:

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251027235858345.png" alt="image-20251027235858345" style="zoom:25%;" />

* ```java
	package Test;
	import java.util.Date;
	public class test {
	    public static void main(String[] args) {
	        //1.创建一个对象, 表示时间原点
	        Date d1 = new Date(0L);
	        System.out.println(d1);//Thu Jan 01 08:00:00 CST 1970
	        //2.获取d1时间的毫秒值
	        long time = d1.getTime();
	        time = time+ 1000L*60*60*24*365;
	        d1.setTime(time);
	        System.out.println(d1);//Fri Jan 01 08:00:00 CST 1971
	    }
	}
	```

* SimpleDateFormat:格式化, 解析

* ```java
	package Test;
	
	import java.text.SimpleDateFormat;
	import java.util.Date;
	
	public class test {
	    public static void main(String[] args) {
	        //空参
	        SimpleDateFormat sdf1 = new SimpleDateFormat();
	        Date d1 = new Date();
	        String str1 = sdf1.format(d1);
	        System.out.println(str1);//2025/10/28 00:20
	
	        //带参
	        SimpleDateFormat sdf2 = new SimpleDateFormat("yyyy年MM月dd日 HH时mm分ss秒");
	        Date d2 = new Date();
	        String str2 = sdf2.format(d2);
	        System.out.println(str2);//2025年10月28日 00时21分22秒
	    }
	}
	```

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251028100042350.png" alt="image-20251028100042350" style="zoom:33%;" />

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251028142154088.png" alt="image-20251028142154088" style="zoom:25%;" />

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251028142339952.png" alt="image-20251028142339952" style="zoom:25%;" />
* 包装类:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251028151819468.png" alt="image-20251028151819468" style="zoom:50%;" />

* 

* ```java
	public class test {
	    public static void main(String[] args) throws ParseException {
	        //1.转换为2进制
	        String str1 = Integer.toBinaryString(100);
	        System.out.println(str1);
	        //2.把整数转成八进制
	        String str2 = Integer.toOctalString(100);
	        System.out.println(str2);
	        //16
	        String str3 = Integer.toHexString(100);
	        System.out.println(str3);
	        //4.字符串转换为int整数
	        int i = Integer.parseInt("100");//只能是数字
	        System.out.println(i);//100
	        String str = "true";
	        boolean bool = Boolean.parseBoolean(str);
	        System.out.println(bool);
	    }
	}
	```

* 习题1

* ```java
	package Test;
	
	import java.text.ParseException;
	import java.text.SimpleDateFormat;
	import java.time.LocalDate;
	import java.time.temporal.ChronoUnit;
	import java.util.Date;
	public class test {
	    public static void main(String[] args) throws ParseException {
	        //计算有多少天
	        String birthday = "1990-01-01";
	        SimpleDateFormat sdf = new SimpleDateFormat("yyyy-MM-dd");
	        Date date = sdf.parse(birthday);
	        long birthdayLong = date.getTime();
	        
	        //2.获取当前时间的毫秒值
	        long todayTime = System.currentTimeMillis();
	        long today = todayTime - birthdayLong;
	        System.out.println(today/1000/60/60/24);
	
	        //JDK8
	        LocalDate d2 = LocalDate.now();
	        LocalDate d1 = LocalDate.of(1990, 1, 1);
	        long days = ChronoUnit.DAYS.between(d1, d2);
	        System.out.println(days);
	    }
	}
	```
	
* 习题2

* ```java
	package Test;
	
	import java.text.ParseException;
	import java.time.LocalDate;
	import java.util.Calendar;
	
	public class test {
	    public static void main(String[] args) throws ParseException {
	        //判断任意一个年份是闰年还是平年
	
	        //JDK7
	        Calendar c = Calendar.getInstance();
	        c.set(2000, 0, 1);//月份范围:0~11
	        c.add(Calendar.DAY_OF_YEAR, -1);
	        int day = c.get(Calendar.DAY_OF_YEAR);
	        System.out.println(day);
	
	        //JDK8
	        LocalDate ld = LocalDate.of(2000,3,1);
	        LocalDate ld2 = ld.minusDays(1);
	        int day2 = ld2.getDayOfMonth();
	        System.out.println(day2);
	
	        System.out.println(ld.isLeapYear());
	    }
	}
	```
	
* Arrays:
  <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029142014630.png" alt="image-20251029142014630" style="zoom:19%;" />

### 8.2.字符串内存分析:

*  <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251021211428203.png" alt="image-20251021211428203" style="zoom:33%;" />

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251021211637981.png" alt="image-20251021211637981" style="zoom:50%;" />

* new:新建一个

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251021211822621.png" alt="image-20251021211822621" style="zoom:50%;" /> 
* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251021212127853.png" alt="image-20251021212127853" style="zoom:25%;" />

* byte[]数组中的转换为字符在进行拼接

### 8.3字符串的相关方法:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251021213555699.png" alt="image-20251021213555699" style="zoom:25%;" />

* substring():包左不包右,包头不包尾

* 

* ```java
	public static String rotate(String str1){
	    char first = str1.charAt(0);
	    String end = str1.substring(1);
	    return end+first;
	}
	```

* charAt(index):

* toCharArray:

* ```java
	public static String rotate(String str1){
	    char[] arr = str1.toCharArray();
	    char first = arr[0];
	    for(int i = 1;i<str1.length();i++){
	        arr[i-1] = arr[i];
	    }
	    arr[str1.length()-1] = first;
	    String result = new String(arr);
	    return result;
	}
	```

* > StringBuilder:
	
	* `一个可变的操作字符串的容器, 可以高效的拼接字符串, 还可以将容器里面的内容进行*反转*(打印的是属性值不是地址值)
	
	* ```java
		package Test;
		import java.util.Scanner;
		public class test {
		    public static void main(String[] args) {
		        Scanner sc = new Scanner(System.in);
		        System.out.println("请输入一个字符串");
		        String str = sc.nextLine();
		
		        String result = new StringBuilder(str).reverse().toString();
		        if(str.equals(result)){
		            System.out.println("该字符串是回文字符串");
		        }else{
		            System.out.println("该字符串不是回文字符串");
		        }
		    }
		}
		```
	
* >StringJoiner

	* JDK8出现的一个可变的操作字符串的容器, 可以高效, 方便的拼接字符串;拼接的时候可以指定间隔`符号, 开始符号, 结束符号

	* ```java
		package Test;
		import java.util.StringJoiner;
		public class test {
		    public static void main(String[] args) {
		        StringJoiner sj = new StringJoiner(", ", "[", "]");
		        sj.add("Hello").add("World").add("Java");
		        System.out.println(sj.toString());//[Hello, World, Java]
		    }
		}
		```









### 8.4小结:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251022151625939.png" alt="image-20251022151625939" style="zoom:25%;" />

## 9.集合:

* 集合和数组的比较:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251022190514900.png" alt="image-20251022190514900" style="zoom:25%;" />

add(), remove(), size(), get()

### 9.1集合的体系结构:

#### <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029161442029.png" alt="image-20251029161442029" style="zoom:25%;" />

#### 9.11单列集合

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251101110055847.png" alt="image-20251101110055847" style="zoom:50%;" />



![image-20251029161525292](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029161525292.png)



##### 9.111 Collection及其遍历:

* 是单列集合的顶层接口, 它的功能是全部单列集合都可以继承使用的.<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029161811084.png" alt="image-20251029161811084" style="zoom:25%;" />

* contains注意:![image-20251029163630946](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029163630946.png)

* > collection的遍历方式:

  * <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029190727517.png" alt="image-20251029190727517" style="zoom:25%;" />

  * > 迭代器遍历

  	1.迭代器在java中的类是Iterator, 迭代器是集合专用的遍历方式

  	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029164126023.png" alt="image-20251029164126023" style="zoom:33%;" />

  	```java
  	package BigInteger;
  	
  	import java.util.ArrayList;
  	import java.util.Collection;
  	import java.util.Iterator;
  	
  	public class Test {
  	    public static void main(String[] args) {
  	        //1.创建集合并添加元素
  	        Collection<String> coll = new ArrayList<>();
  	        coll.add("aaa");
  	        coll.add("bbb");
  	        coll.add("ccc");
  	        //2.获取迭代器对象
  	        //迭代器就好比是一个箭头, 默认指向集合的0索引处
  	        //3.使用迭代器遍历集合
  	        Iterator<String> iterator = coll.iterator();
  	        while (iterator.hasNext()) {
  	            //4.next方法的作用: 1.移动指针(箭头) 2.返回当前指针指向的元素
  	            String str = iterator.next();
  	            System.out.println(str);
  	        }
  	    }
  	}
  	```

  	![image-20251029170745777](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029170745777.png)

  * > 增强for遍历:

  	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029184759744.png" alt="image-20251029184759744" style="zoom:25%;" />

  	

  	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029184904226.png" alt="image-20251029184904226" style="zoom:33%;" />

  	 修改增强for中的变量, 不会改变集合中原本的数据.

  * > lambda表达式遍历:

  	* 得益于JDK8开始的新技术lambda表达式, 提供了一种更简单更直接的遍历集合的方式
  	* 使用前提:接口必须是函数式接口@FunctionalInterface
  	* 遍历方式:先利用匿名内部类的方式, 再修改为lambda表达式
  	* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251031165639228.png" alt="image-20251031165639228" style="zoom:35%;" />
  	  * new创建的不是Consumer接口的对象, 而是后面的没有名字的对象,
  	  * 没有名字的类是实现了Consumer接口, 所以说要在类当中重写接口里面的抽象方法accept
  	* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251031165822144.png" alt="image-20251031165822144" style="zoom: 25%;" />
  	
  	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029185749450.png" alt="image-20251029185749450" style="zoom:33%;" />
  	

##### 9.112List中的常见方法:

* 

```java
package BigInteger;

import java.util.ArrayList;
import java.util.List;

public class Test {
    public static void main(String[] args) {
        List<String> list = new ArrayList<>();
        //2.添加元素
        list.add("hello");
        list.add("world");
        list.add("java");
        //细节:原来索引上的元素会依次往后移动
        list.add(1, "qqq");
        System.out.println(list);//[hello, qqq, world, java]
        //3.删除元素
        list.remove(1);//删除索引为1的元素
        System.out.println(list);//[hello, world, java]    
    }
}
```

* 五种遍历方式的对比:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029195325103.png" alt="image-20251029195325103" style="zoom: 80%;" />


```java
package BigInteger;

import java.util.ArrayList;
import java.util.Iterator;
import java.util.List;
import java.util.ListIterator;

public class Test {
    public static void main(String[] args) {
        List<String> list = new ArrayList<>();
        //2.添加元素
        list.add("hello");
        list.add("world");
        list.add("java");
        //1.迭代器
        Iterator<String>  iterator = list.iterator();
        while (iterator.hasNext()) {
            String next = iterator.next();
            System.out.println(next);
        }
        //2.增强for
        for (String s : list) {
            System.out.println(s);
        }
        //3.lambda表达式
        list.forEach(s -> System.out.println(s));
        //4.普通for循环
        for (int i = 0; i < list.size(); i++) {
            System.out.println(list.get(i));
        }
        //5.列表迭代器
        ListIterator<String> it = list.listIterator();
        while (it.hasNext()) {
            String next = it.next();
            if(next.equals("world")){
                it.add("java");
            }
        }
    }
}
```

##### 9.113  set系列集合:

*   特点

	*  无序:存取顺序不一致
	* 不重复:可以去除重复 
	* 无索引: 没有带索引的方法, 所以不能使用普通for循环遍历, 也不能通过索引来获取元素

*   set是一个接口, 继承于Collection, 方法基本上与Collection的API一致.

*   <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251031114501164.png" alt="image-20251031114501164" style="zoom:33%;" />

* ```java
	package Test;
	
	import java.util.HashSet;
	import java.util.Set;
	
	public class test {
	    public static void main(String[] args) {
	        //1.创建一个Set集合(多态)
	        Set<String> s = new HashSet<>();
	        //2.添加元素
	        boolean a = s.add("hello");
	        boolean b = s.add("hello");
	        System.out.println(a);//true
	        System.out.println(b);//false
	        System.out.println(s);//[hello]
	        //打印出来的是无序的
	    }
	}
	```

*   > HashSet(数据去重默认hashset):

	*   HashSet集合底层采取哈希值存储数据

	* 哈希表

		* 是一种对于增删改查数据性能都较好的结构
		* 组成: JDK8以前是数组+链表; JDK8开始是数组+链表+红黑树(->没有索引)

	* 哈希值:对象的整数表现形式

		* 哈希表在底层是有数组存在的, 根据公式确定要添加数据应存入的位置![image-20251031144718178](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251031144718178.png)

		* 根据hashCode方法算出来的int类型的整数; 该方法定义在Object类中, 所有对象都可以调用, 默认使用地址值进行计算;  一般情况下会重写hashCode, 利用对象内部的属性值计算哈希值

		*  对象哈希值的特点: <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251031145434301.png" alt="image-20251031145434301" style="zoom:33%;" />

		* 使用样

			```java
			package Test;
			
			import java.util.Objects;
			
			public class test {
			    public static void main(String[] args) {
			        //1.创建对象
			        Student s1 = new Student("张三", 18);
			        Student s2 = new Student("张三", 18);
			        //2.如果没有重写hashCode方法, 不同对象计算出的哈希值是不同的
			        System.out.println(s1.hashCode());//24022538
			        System.out.println(s2.hashCode());//24022538
			        //String类中已经重写了hashCode方法, 所以字符串对象的哈希值是根据字符串的内容计算出来的
			        System.out.println("abc".hashCode());//96354
			        System.out.println("acD".hashCode());//96354
			    }
			}
			class Student{
			    private String name;
			    private int age;
			
			    public Student() {
			    }
			
			    public Student(String name, int age) {
			        this.name = name;
			        this.age = age;
			    }
			
			    public String getName() {
			        return name;
			    }
			
			    public void setName(String name) {
			        this.name = name;
			    }
			
			    public int getAge() {
			        return age;
			    }
			
			    public void setAge(int age) {
			        this.age = age;
			    }
			
			    @Override
			    public boolean equals(Object o) {
			        if (o == null || getClass() != o.getClass()) return false;
			        Student student = (Student) o;
			        return age == student.age && Objects.equals(name, student.name);
			    }
			
			    @Override
			    public int hashCode() {
			        return Objects.hash(name, age);
			    }
			    @Override
			    public String toString() {
			        return "Student{" +
			                "name='" + name + '\'' +
			                ", age=" + age +
			                '}';
			    }
			}
			```

	* HashSet底层原理:   <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251031152646624.png" alt="image-20251031152646624" style="zoom:25%;" />存和取的顺序不一样

		![image-20251031153203790](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251031153203790.png)*重写hashCode目的是我们想要根据属性值计算哈希值, 重写equals目的是在比较的时候比的是对象内部的属性值*

		HashSet的去重机制:    hashCode得到哈希值, 哈希值确定当前元素添加在哪个位置, equals去比较对象内部的属性值是否相同

		```java
		package Test;
		
		import java.util.HashSet;
		import java.util.Objects;
		
		public class test {
		    public static void main(String[] args) {
		        //1.创建对象
		        Student s1 = new Student("张三", 18);
		        Student s2 = new Student("李四", 19);
		        Student s3 = new Student("张三", 18);
		
		        HashSet<Student> set = new HashSet<>();
		        System.out.println(set.add(s1));//true
		        System.out.println(set.add(s2));//true
		        System.out.println(set.add(s3));//false因为重写了equals和hashcode方法
		        System.out.println(set);//[Student{name='张三', age=18}, Student{name='李四', age=19}]
		    }
		}
		class Student{
		    private String name;
		    private int age;
		
		    public Student() {
		    }
		
		    public Student(String name, int age) {
		        this.name = name;
		        this.age = age;
		    }
		
		    public String getName() {
		        return name;
		    }
		
		    public void setName(String name) {
		        this.name = name;
		    }
		
		    public int getAge() {
		        return age;
		    }
		
		    public void setAge(int age) {
		        this.age = age;
		    }
		
		    @Override
		    public boolean equals(Object o) {
		        if (o == null || getClass() != o.getClass()) return false;
		        Student student = (Student) o;
		        return age == student.age && Objects.equals(name, student.name);
		    }
		
		    @Override
		    public int hashCode() {
		        return Objects.hash(name, age);
		    }
		    @Override
		    public String toString() {
		        return "Student{" +
		                "name='" + name + '\'' +
		                ", age=" + age +
		                '}';
		    }
		}
		
		```

*  > LinkedHashSet底层原理(要求去重且存取有序):

	* 有序(存储和取出的元素顺序一致),不重复, 无索引
	*  原理:底层数据结构依然哈希表, 只是每个元素又额外的多了一个双链表的机制记录存储的顺序<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251031160322130.png" alt="image-20251031160322130" style="zoom:25%;" />

* > TreeSet:基于红黑树的数据结构实现的, 增删改查性能都较好

	* TreeSet集合默认的规则:对于数值类型, integer, Double, 默认按照从小到大的顺序进行排序, 对于字符, 字符串类型, 按照字符在ASCII码表中的数字升序进行排序
	
	* 两种比较方式:
	
		* ①*默认排序/自然排序*(默认):Javabean类实现Comparable接口, 重写里面的抽象方法, 再指定比较规则
	
		* ```java
			package Test;
			import java.util.TreeSet;
			
			public class test {
			    public static void main(String[] args) {
			        //1.创建对象
			        Student s1 = new Student("zhangsan", 23);
			        Student s2 = new Student("lisi", 24);
			        Student s3 = new Student("wangwu", 25);
			
			        TreeSet<Student> treeSet = new TreeSet<>();
			        treeSet.add(s1);
			        treeSet.add(s2);
			        treeSet.add(s3);
			        //lambda
			        treeSet.forEach(student -> System.out.println(student));
			    }
			}
			class Student implements Comparable<Student> {
			    private String name;
			    private int age;
			    public Student() {
			    }
			    public Student(String name, int age) {
			        this.name = name;
			        this.age = age;
			    }
			    public String getName() {
			        return name;
			    }
			    public void setName(String name) {
			        this.name = name;
			    }
			    public int getAge() {
			        return age;
			    }
			    public void setAge(int age) {
			        this.age = age;
			    }
			    //TreeSet底层不是哈希表, 底层是红黑树结构, 不需要重写hashCode和equals方法
			    @Override
			    public String toString() {
			        return "Student [name=" + name + ", age=" + age + "]";
			    }
			    public int compareTo(Student o) {
			        System.out.println("-------------");
			        System.out.println("this: " + this);//this:表示当前要添加的元素
			        System.out.println("o: " + o);//o:表示已经再红黑树存在的元素
			        //按照年龄的升序进行排列
			        /*(先从根节点开始比较)
			           负数:认为要添加的元素是小的, 存左边
			            0:认为要添加的元素和集合中的元素相等, 不存
			        正数:认为要添加的元素是大的, 存右边
			        结合红黑规则*/
			        return this.age - o.age;
			    }
			}
			```
	
		* ②*比较器排序*(不想按照默认顺序排序): 创建TreeSet对象时候, 传递比较器Comparator指定规则
	
			```java
			package Test;
			import java.util.TreeSet;
			public class test {
			    public static void main(String[] args) {
			        //1.创建对象匿名内部类
			        TreeSet<String> ts = new TreeSet<>((o1, o2)->{
			                int i = o1.length()-o2.length();
			                return i==0?o1.compareTo(o2):i;//如果一样长则按照首字母排序
			        });
			        ts.add("zhangsan");
			        ts.add("lisi");
			        ts.add("wangwu");
			        System.out.println(ts);//负数存左边
			    }
			}
			```
	
			* 注意:先按照长度排(自己指定的方法②的规则), 长度一样再按照首字母排(String类已经有java定义好的默认排序规则方式①), 所以两种方式同时存在时优先方式②



#### 9.12双列集合:

![image-20251101161724618](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251101161724618.png)



##### 9.121特点:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251101111206438.png" alt="image-20251101111206438" style="zoom:40%;" />

* 双列集合一次需要存一对数据, 分别为键和值
* 键不能重复,值可以重复
* 键和值是一一对应的, 每一个键只能找到自己对应的值
* 键+值这个整体, 我们称之为“键值对”或者“键值对对象”,在java中叫做“Entry对象” 

##### 9.122Map:

###### 1.Map的常见API:

```java
package Test;
import java.text.ParseException;
import java.util.HashMap;
import java.util.Map;

public class test {
    public static void main(String[] args) throws ParseException {
        //1.创建Map集合对象
        Map<String, String> m = new HashMap<>();
        //2.添加元素
        //put方法细节:添加元素时,如果键不存在, 那么直接把键值对对象添加到map方法中, 方法返回null
        //            如果键存在, 那么用新值替换旧值, 方法返回的是被替换的旧值
        String value1 = m.put("bbb", "222");
        System.out.println(value1);//null
        m.put("aaa", "111");
        String value2 = m.put("aaa", "333");
        System.out.println(value2);//111
        System.out.println(m);//{aaa=333, bbb=222}
        //删除
        System.out.println(m.remove("aaa"));//333
        //m.clear();
        //System.out.println(m);//{}

        //判断是否包含
        System.out.println(m.containsKey("bbb"));//true
        System.out.println(m.containsValue("222"));//true
        //判断是否为空
        System.out.println(m.isEmpty());//false
    }
}
```

###### 2.Map的遍历方式

* > 键找值:

	```java
	package Test;
	
	import java.util.HashMap;
	import java.util.Map;
	import java.util.Set;
	public class test {
	    public static void main(String[] args){
	        //1.创建Map集合对象
	        Map<String, String> m = new HashMap<>();
	        //2.添加元素
	        m.put("key1", "value1");
	        m.put("key2", "value2");
	        //3.通过键获取值
	        //3.1获取所有的键, 把这些键放到一个单列集合当中
	        Set<String> keys = m.keySet();
	        //3.2遍历所有的键
	        for(String key : keys){
	            String value = m.get(key);
	            System.out.println(key + "=" + value);
	        }
	    }
	}
	```
	
* > 键值对:

	* ```java
		package Test;
		
		import java.util.HashMap;
		import java.util.Map;
		import java.util.Set;
		
		public class test {
		    public static void main(String[] args){
		        Map<String,String> map = new HashMap<>();
		        map.put("key1","value1");
		        map.put("key2","value2");
		        map.put("key3","value3");
		        //通过一个方法获取所有的键值对对象, 返回一个Set集合
		        Set<Map.Entry<String, String>> entries = map.entrySet();
		        //遍历Set集合, 得到每一个键值对对象
		        for (Map.Entry<String, String> entry : entries) {
		            System.out.println(entry.getKey()+"="+entry.getValue());
		        }
		    }
		}
		```

* > lambda表达式遍历

	* ```java
		package Test;
		
		import java.util.HashMap;
		import java.util.Map;
		import java.util.function.BiConsumer;
		
		public class test {
		    public static void main(String[] args){
		        Map<String,String> map = new HashMap<>();
		        map.put("key1","value1");
		        map.put("key2","value2");
		        map.put("key3","value3");
		        //通过一个方法获取所有的键值对对象, 返回一个Set集合
		        map.forEach(new BiConsumer<String, String>() {
		            @Override
		            public void accept(String key, String value) {
		                System.out.println(key+"="+value);
		            }
		        });
		        System.out.println("-------------------------------------");
		        map.forEach((key,value)-> System.out.println(key+"="+value));
		    }
		}
		```

###### 3.HashMap

* > 特点:

	* HashMap是Map里面的一个实现类
	* 没有额外需要学习的特有方法, 直接使用Map里面的方法就可以了
	* 特点都是由键决定:无序,不重复, 无索引
	* HashMap跟HashSet底层原理是一模一样的, 都是哈希表结构, 依赖hashCode方法和equals方法保证*键的唯一*
	* 如果键存储的是自定义对象, 需要重写hashCode方法, 如果值存储自定义对象, 不需要重写hashCode和equals方法

* ![image-20251101143824412](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251101143824412.png)



* > 练习

```java
package Test;
import java.util.*;
public class test {
    public static void main(String[] args) {
        /*80人投票去ABCD四个景点*/
        String[] arr = {"A", "B", "C", "D"};
        ArrayList<String> list = new ArrayList<>();
        Random r = new Random();
        // 随机添加80个元素到list中
        for (int i = 0; i < 80; i++) {
            list.add(arr[r.nextInt(arr.length)]);
        }
        //创建双列集合
        HashMap<String, Integer> map = new HashMap<>();
        //遍历list
        for (String key : list) {
            if (map.containsKey(key)) {
                map.put(key, map.get(key) + 1);
            } else {
                map.put(key, 1);
            }
        }
        //求最大值
        int max = 0;
        Set<Map.Entry<String, Integer>> set = map.entrySet();
        for (Map.Entry<String, Integer> entry : set) {
            if (entry.getValue() > max) {
                max = entry.getValue();
            }
        }
        //4.判断哪个景点的次数跟最大值一样,如果一样, 输出景点名称
        for (Map.Entry<String, Integer> entry : set) {
            if (entry.getValue() == max) {
                System.out.println(entry.getKey());
                System.out.println(max);
            }
        }
    }
}

```

* > LinkedHashMap:

* 特点:

	* 由键决定:*有序*, 不重复, 无索引
	* 这里的有序指的是保证存储和取出的元素顺序一致
	* 原理: 底层数据结构依然是哈希表, 只是每个键值对元素又额外的多了一个双链表的机制记录存储的顺序![image-20251101162455751](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251101162455751.png)

* >HashMap源码分析

	* ctrl+b, ctrl+f12![image-20251101192029348](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251101192029348.png)

​			<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251101193240601.png" alt="image-20251101193240601" style="zoom:50%;" />

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251101193612679.png" alt="image-20251101193612679" style="zoom:35%;" />



ctrl+alt+左键:回到上一步



###### 4.TreeMap:

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251101163119872.png" alt="image-20251101163119872" style="zoom: 33%;" />默认第一种:java事先设定好的

```java
package Test;
import java.util.StringJoiner;
import java.util.TreeMap;
public class test {
    public static void main(String[] args) {
        //利用map集合进行统计,如果没有要求对结果进行排序,就用HashMap
        //如果有要求对结果进行排序,就用TreeMap
        String s = "aababcabcdabcde";
        TreeMap<Character,Integer> map = new TreeMap<>();
        //遍历
        for (int i = 0; i < s.length(); i++) {
            char c = s.charAt(i);
            if(map.containsKey(c)){
                Integer count = map.get(c);
                count++;
                map.put(c, count);
            }else{
                map.put(c, 1);
            }
        }
        //1.直接遍历拼接
        String result = "";
        for(Character key : map.keySet()){
            result = result + key + "(" +map.get(key)+")";
        }
        //2.StringBuilder
        //利用StringBuilder进行拼接
        StringBuilder sb = new StringBuilder();
        map.forEach((key,value)->sb.append(key).append("(").append(value).append(")"));
        System.out.println(sb);
        //3.StringJoiner
        //利用StringJoiner进行拼接
        StringJoiner sj = new StringJoiner("", "", "");
        map.forEach((key,value)->sj.add(key+"("+value+")"));
        System.out.println(sj);
    }
}
```

###### 5.三种总结问题

* TreeMap添加元素的时候, 键是否需要重写hashCode和equals方法?
	* 此时是不需要重写的, TreeMap 基于红黑树实现，通过键的比较来维护元素顺序，而不是像 HashMap 那样通过哈希码。<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251101215510355.png" alt="image-20251101215510355" style="zoom:33%;" />

* HashMap是哈希表结构的, JDK8开始由数组, 链表, 红黑树组成的, 既然有红黑树, HashMap的键是否需要实现Compareable接口或者传递比较器对象呢?
	* 不需要, 因为在HashMap的底层, 默认是利用哈希值的大小关系来创建红黑树的



* TreeMap和HashMap谁的效率更高?
	* 如果是最坏情况, 添加了8个元素, 这8个元素形成了链表, 此时TreeMap的效率更高, 但是这种情况出现的几率非常少. 一般而言, 还是HashMap的效率要更高
* 在Map集合中, java会提供一个如果键重复了, 不会覆盖的put方法呢?
	* putIfAbsent<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251102125305677.png" alt="image-20251102125305677" style="zoom: 33%;" />
	* 传递一个思想:代码中的逻辑都有两面性, 如果我们只知道了其中的A面, 而且代码中还发现了有变量可以控制两面性的发生, 那么该逻辑一定会有B面
	* 习惯: Boolean类型的变量控制, 一般只有AB两面, 因为boolean只有两个值, int类型的变量控制, 一般至少有三面, 因为int可以取多个值.


* 三种双列集合, 以后如何选择?
	* 默认:HashMap
	* 如果要保证存取有序:LinkedHashMap
	* 如果要进行排序: TreeMap





### 9.2数据结构:

* 栈

* 队列

* 数组:
  * 查询速度块, 删除效率低, 添加效率极低
  * 在内存当中是一片连续的空间

* 链表:
  * 节点是独立的对象, 在内存中是不连续的, 每个结点包含数据值和下一个结点的地址
  * 查询慢, 增删快,首尾操作极快

* 树:

	* 二叉树
	  * 二叉查找树:减小二叉树查找效率低的弊端
	  	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030202546641.png" alt="image-20251030202546641" style="zoom:33%;" />

	* 二叉树的遍历方式:

	  * 前序遍历:当前在前面<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030203258046.png" alt="image-20251030203258046" style="zoom:30%;" />

	  * 中序遍历:当前在中间

	  	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030203440080.png" alt="image-20251030203440080" style="zoom:50%;" />

	  * 后序遍历:当前在后面
	  	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030203639681.png" alt="image-20251030203639681" style="zoom:20%;" />

	  * 层序遍历:
	  	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030203726565.png" alt="image-20251030203726565" style="zoom:25%;" />

	* 平衡二叉树:任意节点左右子树高度差不超过1, 避免长短腿的出现
	  * <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030204407247.png" alt="image-20251030204407247" style="zoom:25%;" />

	* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030204910085.png" alt="image-20251030204910085" style="zoom:25%;" />

	* 平衡二叉树的旋转机制:平衡二叉树是通过旋转机制保持平衡的;

	  * <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030205322764.png" alt="image-20251030205322764" style="zoom:25%;" />

	  * 1.左旋:
	  	左旋请况1:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030205954504.png" alt="image-20251030205954504" style="zoom:25%;" />

​					左旋情况2:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251031094836225.png" alt="image-20251031094836225" style="zoom:25%;" />





​						2.右旋

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030212341607.png" alt="image-20251030212341607" style="zoom:19%;" />



<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030212424477.png" alt="image-20251030212424477" style="zoom:20%;" />



​															旋转情况的总结:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030215359786.png" alt="image-20251030215359786" style="zoom:15%;" />	

* 红黑树:

	* > 它是一种特殊的二叉查找树, 红黑树的每一个节点上都有存储位表示节点的颜色.
	* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251031102623922.png" alt="image-20251031102623922" style="zoom: 33%;" />
	* > 红黑规则:
		
		* 每一个节点或是红色的, 或者是黑色的
		* 根节点必须是黑色
		* 如果一个节点*没有子节点或者父节点*, 则该节点相应的指针属性值为Nil, 这些Nil视为叶节点, 每个叶节点(Nil)是黑色的
		* 如果一个节点是红色, 那么它的子节点必须是黑色  *(不能出现两个红色节点相连的情况)*
		* 对每一个节点, 从该节点到其所有后代叶节点的简单路径上, 均包含相同数目的黑色节点
		* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251031103509129.png" alt="image-20251031103509129" style="zoom:25%;" /><img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251031103528627.png" alt="image-20251031103528627" style="zoom:39%;" />
	
	
	
	
	
	* 添加节点规则:
		* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251031105323735.png" alt="image-20251031105323735" style="zoom:15%;" />
	* 





### 9.3ArrayList和LinkedList和迭代器源码分析:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029204439503.png" alt="image-20251029204439503" style="zoom:25%;" />

ArrayList:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029214449975.png" alt="image-20251029214449975" style="zoom:25%;" />



双向链表:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030115522073.png" alt="image-20251030115522073" style="zoom:19%;" />

迭代器:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030135101366.png" alt="image-20251030135101366" style="zoom: 20%;" />

### 9.4泛型:

* 泛型概述:

	* 是JDK5中引入的特性, 可以在编译阶段约束操作的数据类型, 并进行检查
	* 泛型的格式:<数据类型>
	* 如果不写泛型, 类型默认是Object
	* 指定泛型的具体类型后, 传递数据时, 可以传入该类或子类(一般时该类)
	* 注意:*泛型只能支持引用数据类型, 不能写基本数据类型*(解决方案是使用对应的包装类)
		* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030144138165.png" alt="image-20251030144138165" style="zoom:33%;" />

* 泛型类

* ```java
	package MyArrayList;
	
	import java.util.Arrays;
	
	public class Demo2 {
	    public static void main(String[] args) {
	        MyArrayList<Integer> list = new MyArrayList<Integer>();
	        list.add(100);
	        list.add(200);
	        list.add(300);
	        System.out.println(list);//[100, 200, 300, null, null, null, null, null, null, null]
	        int i = list.get(0);
	        System.out.println(i);//100
	    }
	}
	class MyArrayList<E> {
	    Object[] obj = new Object[10];
	    int size;
	    //E:表示不确定的类型,
	    public boolean add(E e){
	        obj[size] = e;
	        size++;
	        return true;
	    }
	
	    //获取元素
	    public E get(int index){
	        return (E)obj[index];
	    }
	
	    public String toString(){
	        return Arrays.toString(obj);
	    }
	}
	```

* 泛型的好处:

	* 统一数据类型
	* 把运行时期的问题提前到了编译期间, *避免了强制类型转换可能出现的异常*, 因为在编译阶段类型就能确定下来
		* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030141337617.png" alt="image-20251030141337617" style="zoom: 33%;" />
			* 数据类型不同不一定能强转, 把123(int)强转成Student会报错

* 泛型方法:

	* 一个类当中, 只有一个方法的形参不确定, 而不是整个类的形参不确定, 可以把泛型定义在方法上面

	* 

	* ```java
		package MyArrayList;
		
		import java.util.ArrayList;
		
		public class demo3 {
		    public static void main(String[] args) {
		        ArrayList<Integer> list = new ArrayList<Integer>();
		        ListUtil.addAll(list, 100, 200);
		        System.out.println(list);
		    }
		}
		class ListUtil<E> {
		    private ListUtil(){}
		
		    //定义一个静态方法addAll, 用来添加多个集合的元素
		    public static<E> void addAll(ArrayList<E> list, E e1, E e2){
		        list.add(e1);
		        list.add(e2);
		    }
		}
		```



* 泛型接口:
	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030155840350.png" alt="image-20251030155840350" style="zoom:25%;" />



<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251030155936899.png" alt="image-20251030155936899" style="zoom:50%;" />

* 泛型的继承和通配符

	* 泛型不具备继承性, 但是数据具备继承性

		

	* ```java
		package MyArrayList;
		
		import java.util.ArrayList;
		
		public class test {
		    public static void main(String[] args) {
		
		        ArrayList<Ye> list1 = new ArrayList<>();
		        ArrayList<Fu> list2 = new ArrayList<>();
		        ArrayList<Zi> list3 = new ArrayList<>();
		
		        //调用method方法，传递list1
		        method(list1);
		        //method(list2);报错, 泛型不具备继承性
		        //method(list3);报错
		
		        //数据具备继承性
		        list1.add(new Ye());
		        list1.add(new Fu());
		        list1.add(new Zi());
		
		    }
		    //此时, 泛型里面写的是什么类型, 那么只能传递什么类型的数据
		    public static void method(ArrayList<Ye> list){
		
		    }
		
		}
		class Ye{
		
		}
		class Fu extends Ye{
		
		}
		class Zi extends Ye{
		
		}
		```

	* 泛型的通配符关键点: 可以限定类型的范围

	* 

	* ```java
		package MyArrayList;
		
		import java.util.ArrayList;
		
		public class test {
		    public static void main(String[] args) {
		
		        ArrayList<Ye> list1 = new ArrayList<>();
		        ArrayList<Fu> list2 = new ArrayList<>();
		        ArrayList<Zi> list3 = new ArrayList<>();
		        ArrayList<Student> list4 = new ArrayList<>();
		
		        //调用method方法，传递list1
		        method(list1);
		        method(list2);
		        method(list3);
		
		
		
		    }
		    //泛型的通配符:
		    //    ? 也表示不确定的类型
		    //    可以进行类型的限定
		    //    ? extends E:表示可以传递E或者E所有的子类类型
		    //    ? super E: 表示可以传递E或者E所有的父类类型
		    /*应用场景:1.如果我们在定义类,方法,接口的时候, 如果类型不确定, 就可以定义泛型类, 泛型方法, 泛型接口.
		              2.如果类型不确定, 但是能知道以后只能传递某个继承体系中的, 就可以泛型的通配符.*/
		    
		    //                                  <? super Zi>
		    public static void method(ArrayList<? extends Ye> list){
		
		    }
		
		}
		class Ye{
		
		}
		class Fu extends Ye{
		
		}
		class Zi extends Ye{
		
		}
		class Student{
		
		}
		```

### 9.5集合工具类Collections:

* > Collections

	* java.util.Collections:是集合工具类
	* 作用:Collections不是集合, 而是集合的工具类

* Collections常用API:

	*  ![image-20251102140649523](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251102140649523.png)

### 9.6不可变集合

* >应用场景:不想让别人修改集合中的内容

	* 如果某个数据不能被修改, 把他防御性地拷贝到不可变集合中是个很好的实践
	* 当集合对象被不可信地库调用时, 不可变形式是安全的

* >书写格式

	* ![image-20251102194409297](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251102194409297.png)



​			细节: list可以直接用, set元素不能重复, map元素不能重复, 键值对数量最多是10个, 超过用ofEntries方法

```java
package Test;

import java.util.HashMap;
import java.util.List;
import java.util.Map;
import java.util.Set;

public class test {
    public static void main(String[] args) {
        List<String> list = List.of("aaa", "bbb", "ccc");
        Map<String, Integer> map1 = Map.of("aaa", 1, "bbb", 2, "ccc", 3);
        Set<String> set = Set.of("aaa", "bbb", "ccc");//注意set里面的元素是不能重复的

        Map<String, Integer> map2 = new HashMap<>();
        map2.put("aaa", 1);
        map2.put("bbb", 2);
        map2.put("ccc", 3);
        map2.put("ddd", 4);
        map2.put("eee", 5);
        map2.put("fff", 6);
        map2.put("ggg", 7);
        map2.put("hhh", 8);
        map2.put("iiii", 9);
        map2.put("jjjj", 10);
        map2.put("kkkk", 11);
        //由map2创建一个不可变的map, 两种方式
        //先转换为数组, 再创建不可变的map, 其中entrySet()返回的是Set<Map.Entry<K, V>>类型, toArray()将其转换为数组
        Map<Object, Object> m = Map.ofEntries(map2.entrySet().toArray(new Map.Entry[0]));
        Map<String, Integer> map3 = Map.copyOf(map2);
        map2.put("llll", 12);
    }
}
```

### 9.7stream流

* >stream流作用

	* 结合了lambda表达式, 简化集合数组的操作

* >使用步骤:

	* 先得到一条stream流(流水线), 并把数据放上去
	* 利用stream流中的api进行各种操作![image-20251102210650396](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251102210650396.png)







* >获取方式

  * <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251102210237406.png" alt="image-20251102210237406" style="zoom:50%;" />

  * ```java
    package Test;
    
    import java.util.ArrayList;
    import java.util.Arrays;
    import java.util.Collections;
    import java.util.HashMap;
    import java.util.stream.Stream;
    
    public class test {
        public static void main(String[] args) {
            //1.单列集合获取stream流
            ArrayList list = new ArrayList();
            Collections.addAll(list, "a", "b", "c");
            list.stream().forEach(s->System.out.println(s));
            list.stream().forEach(System.out::println);
            //2.双列集合转换成stream流
            HashMap<Integer,String> map = new HashMap<>();
            map.put(1,"a");
            map.put(2,"b");
            map.put(3,"c");
            //方法一:键流
            map.keySet().stream().forEach(s-> System.out.println(s));
            //方法2:键值对流
            map.entrySet().stream().forEach(s-> System.out.println(s));
            //3.数组
            int[] arr = {1, 2, 3, 4, 5, 6, 7, 8};
            Arrays.stream(arr).forEach(s-> System.out.println(s));
            String[] str = {"a", "b", "c"};
            Arrays.stream(str).forEach(s-> System.out.println(s));
            //4.一堆零散数据
            Stream.of("a","b","c").forEach(s-> System.out.println(s));
            //Stream接口中静态方法of细节
            //方法的形参是一个可变参数, 可以传递一堆零散的数据, 也可以传递数组
            //但是数组必须是引用数据类型, 如果是基本数据类型, 是会把整个数组当作一个元素, 放到Stream当中
            Stream.of(arr).forEach(s-> System.out.println(s));//[I@65b54208, 因为arr是数组,所以打印的是数组的地址
            Stream.of(str).forEach(s-> System.out.println(s));
        }
    }
    ```

* >stream流中的方法

	* 中间方法

		* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251103165317051.png" alt="image-20251103165317051" style="zoom: 33%;" />

		* 

			```java
			package Test;
			
			import java.util.ArrayList;
			import java.util.Collections;
			import java.util.function.Function;
			import java.util.stream.Stream;
			
			public class test {
			    public static void main(String[] args) {
			        ArrayList<String> list = new ArrayList<>();
			        Collections.addAll(list, "aaa", "abb", "ccc", "ddd", "ddd");
			        //1.filter
			        list.stream().filter(s->s.startsWith("a"))
			                     .forEach(s->System.out.print(s+" "));//aaa abb
			        System.out.println();
			        //2.limit获取前几个元素
			        list.stream().limit(2)
			                     .forEach(s->System.out.print(s+" "));//aaa abb
			        System.out.println();
			        //3.skip跳过前几个元素
			        list.stream().skip(2)
			                     .forEach(s->System.out.print(s+" "));//ccc ddd ddd
			        System.out.println();
			        //获取abb和ccc
			        list.stream().skip(1)
			                     .limit(2)
			                     .forEach(s->System.out.print(s+" "));//abb ccc
			        System.out.println();
			        //4.distinct去重
			        list.stream().distinct()
			                     .forEach(s->System.out.print(s+" "));//aaa abb ccc ddd
			        System.out.println();
			        //5.concat合并流
			        ArrayList<String> list2 = new ArrayList<>();
			        Collections.addAll(list2, "eee", "fff", "ggg");
			        Stream.concat(list.stream(), list2.stream())
			                     .forEach(s->System.out.print(s+" "));//aaa abb ccc ddd ddd eee fff ggg
			        System.out.println();
			        //6.map
			        ArrayList<String> list3 = new ArrayList<>();
			        Collections.addAll(list3, "zhangsan-23", "lisi-24", "wangwu-25");
			        list3.stream().map(s->s.split("-")[1])
			                     .forEach(s->System.out.println(Integer.parseInt(s)));//将s转换为整数
			        //
			        list3.stream().map(new Function<String, Integer>() {
			                    @Override
			                    public Integer apply(String s) {
			                        return Integer.parseInt(s.split("-")[1]);
			                    }
			        }).forEach(s->System.out.println(s));
			    }
			}
			```

		* 

		* ```java
			package Test;
			import java.util.ArrayList;
			import java.util.Collections;
			import java.util.List;
			import java.util.stream.Collectors;
			import java.util.stream.Stream;
			
			public class test {
			    public static void main(String[] args) {
			        ArrayList<String> manList = new ArrayList<>();
			        Collections.addAll(manList, "张三撒,23", "李四,24", "王五,25", "亲戚,27", "飒飒的,45", "当实时,67");
			        ArrayList<String> femaleList = new ArrayList<>();
			        Collections.addAll(femaleList, "杨三三,23", "杨四三,24", "杨五三,25", "赵六三,26", "看了看,32", "撒啊说,33");
			        List<Actor> actors =Stream.concat(manList.stream()
			                        .filter(s -> s.split(",")[0].length() == 3)
			                        .limit(2)
			                , femaleList.stream()
			                        .filter(s -> s.startsWith("杨"))
			                        .skip(1)
			        ).map(s->new Actor(s.split(",")[0], Integer.parseInt(s.split(",")[1])))
			                .collect(Collectors.toList());
			        actors.forEach(System.out::println);
			    }
			}
			class Actor{
			    private String name;
			    private int age;
			    public Actor(String name, int age) {
			        this.name = name;
			        this.age = age;
			    }
			    public String getName() {
			        return name;
			    }
			    public void setName(String name) {
			        this.name = name;
			    }
			    public int getAge() {
			        return age;
			    }
			    public void setAge(int age) {
			        this.age = age;
			    }
			    @Override
			    public String toString() {
			        return "Actor{" +
			                "name='" + name + '\'' +
			                ", age=" + age +
			                '}';
			
			    }
			}
			```

	* 终结方法

		*  <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251103184454172.png" alt="image-20251103184454172" style="zoom:50%;" />

		* ```java
			package Test;
			import java.util.*;
			import java.util.function.Consumer;
			import java.util.function.Function;
			import java.util.function.IntFunction;
			import java.util.stream.Collectors;
			public class test {
			    public static void main(String[] args) {
			        ArrayList<String> list = new ArrayList<>();
			        Collections.addAll(list, "aaa", "abb", "ccc", "ddd", "ddd");
			        list.stream().forEach(new Consumer<String>() {
			            @Override
			            public void accept(String s) {
			                System.out.println(s);
			            }
			        });
			        list.stream().forEach(s -> System.out.println(s));
			        //统计
			        long count = list.stream().count();
			        System.out.println(count);
			        //收集流中的数组, 放到数组中
			        String[] strings = list.stream().toArray(new IntFunction<String[]>() {
			            @Override
			            public String[] apply(int value) {
			                return new String[value];
			            }
			        });
			        System.out.println(Arrays.toString(strings));
			        
			        //放到集合
			        ArrayList<String> list1 = new ArrayList<>();
			        Collections.addAll(list1, "zhangsan-23", "lisi-24", "wangwu-25");
			        //放到集合中
			        // Set和List
			        Set<String> set = list1.stream().collect(Collectors.toSet());//会对元素去重
			        System.out.println(set);//[zhangsan-23, wangwu-25, lisi-24]
			        List<String> list2 = list1.stream().collect(Collectors.toList());
			        System.out.println(list2);//[zhangsan-23, lisi-24, wangwu-25]
			        // Map
			        Map<String, Integer> map = list1.stream().collect(Collectors.toMap(new Function<String, String>() {
			            @Override
			            public String apply(String s) {
			                return s.split("-")[0];
			            }
			        }, new Function<String, Integer>() {
			            @Override
			            public Integer apply(String s){
			                return Integer.parseInt(s.split("-")[1]);
			            }
			        }));
			        System.out.println(map);//{lisi=24, zhangsan=23, wangwu=25}
			        //labmbda
			        Map<String, Integer> map1 = list1.stream().collect(Collectors.toMap(s -> s.split("-")[0], s -> Integer.parseInt(s.split("-")[1])));
			        System.out.println(map1);//{lisi=24, zhangsan=23, wangwu=25}
			    }
			}
			```





## 10.面向对象进阶:

### 10.1static和静态方法

* 内存图 <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251023165140941.png" alt="image-20251023165140941" style="zoom:20%;" />

* 静态区是内存中共享的,谁要谁去拿
* 被static修饰的成员变量是静态变量,*被该类所有对象共享,随着类的加载而加载,优先于对象存在*
* 推荐类名调用而不是对象名调用

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251023165813527.png" alt="image-20251023165813527" style="zoom:25%;" />

* 工具类:
	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251023170005818.png" alt="image-20251023170005818" style="zoom:30%;" />

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251023182801078.png" alt="image-20251023182801078" style="zoom: 80%;" />

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251023183130553.png" alt="image-20251023183130553" style="zoom:19%;" />

### 10.2:继承

* 定义:提出共性内容

*   <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251023185609564.png" alt="image-20251023185609564" style="zoom:30%;" />

* 当类与类之间,存在相同(共性)的内容, 并满足子类是父类的一种, 就可以考虑使用继承, 来优化代码
* 格式:  <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251023190152974.png" alt="image-20251023190152974" style="zoom:33%;" />

* 特点:  一个子类只能继承一个父类, 子类不能同时继承多个父类.但是支持多层继承
* Object类相当于头头
* 继承的内存图:

	* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251023195349448.png" alt="image-20251023195349448" style="zoom:25%;" />

	* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251023195450477.png" alt="image-20251023195450477" style="zoom:25%;" />

* 规则:
  * 成员变量:非私有的子类可以使用, private的虽然继承下来但不能直接使用

  	* 访问是就近原则

  * 构造方法:

  	* 不能继承:

  	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251023201019481.png" alt="image-20251023201019481" style="zoom:25%;" />

  	* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251023213343007.png" alt="image-20251023213343007" style="zoom:25%;" />

  * 成员方法:
  	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251023200602176.png" alt="image-20251023200602176" style="zoom:15%;" />

  	* 虚方法:非private  非final  非static,可以继承
  	* 就近原则

* 方法的重写:

	* 子类覆盖了父类虚方法表中的方法
	* 
	* ```java
		package ObjectTest;
		
		public class ObjectDemo1 {
		    public static void main(String[] args) {
		
		        //1.toString 返回对象的字符串形式
		        Object obj = new Object();
		        String str1 = obj.toString();
		        System.out.println(str1);//java.lang.Object@27716f4
		
		        Student stu =  new Student();
		        String str2 = stu.toString();
		        System.out.println(str2);//null, 0
		        stu.setAge(12);
		        stu.setName("zhangsan");
		        System.out.println(stu);//zhangsan, 12
		    }
		}
		class Student {
		    private String name;
		    private int age;
		
		    public Student() {
		
		    }
		    public Student(String name, int age) {
		        this.name = name;
		        this.age = age;
		    }
		
		    public String getName() {
		        return name;
		    }
		
		    public void setName(String name) {
		        this.name = name;
		    }
		
		    public int getAge() {
		        return age;
		    }
		
		    public void setAge(int age) {
		        this.age = age;
		    }
		    //重写父类object中的toString
		    public String toString(){
		        return name+", "+age;
		    }
		}
		```
	
	* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251023210143785.png" alt="image-20251023210143785" style="zoom:25%;" />
	
	* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251023210858955.png" alt="image-20251023210858955" style="zoom:25%;" />

### 10.3this和super:

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251023215055713.png" alt="image-20251023215055713" style="zoom:25%;" />

* this访问本类的解释:
	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251023215147941.png" alt="image-20251023215147941" style="zoom: 33%;" />
	* this()和super()一样必须要写在第一行

### 10.4多态:

* 使用父类作为参数,可以接受所有的子类对象

* 调用成员变量:编译看左边,运行也看左边

* 调用成员方法:编译看左边,运行看右边

* ```java
	package demo3;
	
	public class Test {
	    public static void main(String[] args) {
	        Teacher teacher = new Teacher("王建国", 30);
	        Student student = new Student("张三", 18);
	        Administer administer = new Administer("王建", 30);
	
	        //多态就是父类引用指向子类对象, 可以调用子类的方法
	        teacher.show();
	        student.show();
	        administer.show();
	    }
	    public static void show(Person person){
	        System.out.println(person.getName()+"的年龄为："+person.getAge());
	    }
	}
	```

* 多态调用成员的内存图解:
	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024154205536.png" alt="image-20251024154205536" style="zoom:25%;" />

* 类型转换:

	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024160319807.png" alt="image-20251024160319807" style="zoom:25%;" />

	* 自动类型转换
	* 强制类型转换

11.5包和final

* 包:就是文件夹

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024172921293.png" alt="image-20251024172921293" style="zoom:33%;" />

* 规则导包:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024173609013.png" alt="image-20251024173609013" style="zoom:35%;" />

	* 需要导包<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024173403598.png" alt="image-20251024173403598" style="zoom:25%;" />

	* 不需要导包(有java.lang):<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024173510987.png" alt="image-20251024173510987" style="zoom:25%;" />

* 全类名:包名+类名
* final<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024183506088.png" alt="image-20251024183506088" style="zoom:25%;" />

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024183656575.png" alt="image-20251024183656575" style="zoom:25%;" />
	* 地址值不变:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024183937241.png" alt="image-20251024183937241" style="zoom:25%;" />

### 10.5权限修饰符和代码块

* 使用说明<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024192803673.png" alt="image-20251024192803673" style="zoom:25%;" />

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024192821709.png" alt="image-20251024192821709" style="zoom:65%;" />

* 代码块:

	* 局部代码块:
		<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024193324028.png" alt="image-20251024193324028" style="zoom:25%;" />
	* 构造代码块:
		* 提取重复的代码
		* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024194105389.png" alt="image-20251024194105389" style="zoom:33%;" />
	* 静态代码块: 数据初始化
	  * 随着类的加载而加载, 并且自动触发, 只执行一次
	  * <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024194841961.png" alt="image-20251024194841961" style="zoom: 33%;" />
	  * 为什么要用静态:   直接写在main()可能被别人调用, 

### 10.6:抽象类和抽象方法:

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024202257789.png" alt="image-20251024202257789" style="zoom:25%;" />

* 抽取共性时,无法确定方法体, 就把方法定义为抽象的
* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024202110910.png" alt="image-20251024202110910" style="zoom:25%;" />

* 定义格式:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024202404525.png" alt="image-20251024202404525" style="zoom:25%;" />

### 10.7接口:

* idea上创建接口文件:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024205105592.png" alt="image-20251024205105592" style="zoom:25%;" />

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024210150788.png" alt="image-20251024210150788" style="zoom:25%;" />

	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024213307997.png" alt="image-20251024213307997" style="zoom:25%;" />

	* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024214409023.png" alt="image-20251024214409023" style="zoom: 33%;" />

	* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024214724328.png" alt="image-20251024214724328" style="zoom:33%;" />



* 私有方法:普通的私有方法, 静态的私有方法

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024210749361.png" alt="image-20251024210749361" style="zoom:25%;" />

	

* 接口和多态:
	1.<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024215534250.png" alt="image-20251024215534250" style="zoom:25%;" />

* 适配器设计模式:在实现类和接口之间添加了第三者
	* ![image-20251025000540025](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251025000540025.png)
	* 设计模式(各种套路)
	* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251025002128088.png" alt="image-20251025002128088" style="zoom:25%;" />
	* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251024220053073.png" alt="image-20251024220053073" style="zoom:33%;" />

### 10.8内部类:

* 类的五大成员之一(属性,方法,构造方法,代码块,内部类)
* 外部想要访问内部类的成员,必须创建对象

* ```Java
	public class Car {
	    String carName;
	    int carAge;
	    String carColor;
	
	    class Engine{
	        String engineName;
	        int engineAge;
	    }
	}
	```

* eg. 汽车的发动机, ArrayList的迭代器, 人的心脏

* 分类:

	* 成员内部类:写在成员位置的,没有用static修饰的

		* 获取格式:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251025103926713.png" alt="image-20251025103926713" style="zoom:33%;" />
			* 如果被private修饰,调用方式<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251025104743343.png" alt="image-20251025104743343" style="zoom:25%;" />
		* 内存图:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251025102843764.png" alt="image-20251025102843764" style="zoom:25%;" />

	* > 静态内部类:只能访问外部类中的静态变量和静态方法, 如果想要访问非静态的需要创建对象

	  
	
	  * 静态内部类使用示例:

	  	```java
	  	package com.itheima.demo1;
	  	
	  	public class OuterTest{
	  	    public static void main(String[] args) {
	  	        // 创建静态内部类实例
	  	        Outer.Inner inner = new Outer.Inner();
	  	        inner.show1();  // 调用实例方法, inner.show2()
	  	
	  	        // 直接调用静态方法
	  	        Outer.Inner.show2();
	  	    }
	  	}
	  	
	  	class Outer {
	  	    int a = 10;
	  	    static int b = 20;
	  	
	  	    // 静态内部类
	  	    static class Inner {
	  	        public void show1() {
	  	            Outer o = new Outer();
	  	            System.out.println(o.a);//10
	  	            System.out.println(b);//20
	  	        }
	  	
	  	        public static void show2() {
	  	            // System.out.println("静态的方法被调用了");
	  	            Outer o = new Outer();
	  	            System.out.println(o.a);//10
	  	            System.out.println(b);//20
	  	        }
	  	    }
	  	}
	  	```
	
	  * 调用静态内部类中的方法:
	  	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251025112348658.png" alt="image-20251025112348658" style="zoom:25%;" />
	
	* 局部内部类:类似方法中的局部变量, public, protected, private不能修饰
	
	* 匿名内部类:
	
		* 隐藏了名字的内部类, 可以写在成员位置, 也可以写在局部位置
		* 格式:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251025115140793.png" alt="image-20251025115140793" style="zoom:25%;" />
	
		* 格式的细节:

## 11.常见算法

#### 11.1排序:

<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251028212221491.png" alt="image-20251028212221491" style="zoom:33%;" />

#### 11.2:lambda表达式:

* > 函数式编程:是一种思想特点, 忽略面向对象的语法;

* > 函数式接口:有且仅有一个抽象方法的接口叫做函数式接口, 接口上方可以加@FunctionalInterface注解

* > lambda表达式是jdk8开始后的一种新语法形式

	* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029142603086.png" alt="image-20251029142603086" style="zoom: 25%;" />

	* *可以简化匿名内部类的书写*
	* *只能简化函数式接口的匿名内部类的写法*
	* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029143754076.png" alt="image-20251029143754076" style="zoom:33%;" />

	* 之前不用lambda表达式

	* ```java
		package BigInteger;
		
		public class Test {
		    public static void main(String[] args) {
		        method(new Swim(){
		            @Override
		            public void swimming() {
		                System.out.println("我会游泳");
		            }
		        });
		    }
		    public static void method(Swim s){
		        s.swimming();
		    }
		}
		interface Swim{
		    public abstract  void swimming();
		}
		```

	* 用lambda表达式

	* ```java
		package BigInteger;
		
		public class Test {
		    public static void main(String[] args) {
		        method(
		                ()->{
		                    System.out.println("我会游泳");
		                }
		        );
		    }
		    public static void method(Swim s){
		        s.swimming();
		    }
		}
		interface Swim{
		    public abstract  void swimming();
		}
		```

	* 省略规则:<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251029145658434.png" alt="image-20251029145658434" style="zoom:25%;" />

		* 

		* ```java
			package BigInteger;
			
			import java.util.Arrays;
			
			public class Test {
			    public static void main(String[] args) {
			        String[] arr = {"a", "aa", "aaaa", "aaa"};
			        /*Arrays.sort(arr, new Comparator<String>() {
			            @Override
			            public int compare(String o1, String o2) {
			                return o1.length() - o2.length();
			            }
			        });*/
			        Arrays.sort(arr, ( o1, o2)-> o1.length() - o2.length());
			
			
			        System.out.println(Arrays.toString(arr));
			    }
			}
			```

		* ```java
			package BigInteger;
			
			import java.util.Arrays;
			import java.util.Comparator;
			
			public class Test {
			    public static void main(String[] args) {
			        Integer[] arr = {1, 3, 2, 5, 7, 6};
			        Arrays.sort(arr, new Comparator<Integer>() {
			            @Override
			            public int compare(Integer o1, Integer o2) {
			                return o1 - o2;
			            }
			        });
			        //lambda表达式
			        Arrays.sort(arr, (o1, o2) -> o2 - o1);
			        System.out.println(Arrays.toString(arr));
			    }
			}
			```

* 题目:

* ```java
	package GF;
	
	import java.util.Arrays;
	
	public class test {
	    public static void main(String[] args) {
	        GirlFriend gf1 = new GirlFriend("gf1", 18, 1.68);
	        GirlFriend gf2 = new GirlFriend("gf2", 19, 1.65);
	        GirlFriend gf3 = new GirlFriend("gf3", 19, 1.70);
	        //2.
	        GirlFriend[] arr = {gf1, gf2, gf3};
	        Arrays.sort(arr, (o1, o2)->{
	                double temp = o1.getAge() - o2.getAge();
	                temp = temp == 0 ? o1.getHeight() - o2.getHeight() : temp;
	                temp = temp == 0 ? o1.getName().compareTo(o2.getName()) : temp;
	                if(temp > 0){
	                    return 1;
	                }else if(temp < 0){
	                    return -1;
	                }else{
	                    return 0;
	                }
	        });
	        System.out.println(Arrays.toString(arr));//先按年龄排序，年龄相同按身高排序，身高相同按姓名排序
	    }
	}
	```

## 12.方法引用:

### 12.1概述:

* >把已有的方法拿过来用, 当作函数式接口中的抽象方法的方法体, 其中方法引用符是::

* >条件

	* 引用处:必须是函数式接口

	* 被引用的方法: 1.被引用的方法必须已经存在

		​						2.被引用方法的形参和返回值需要跟抽象方法保持一致<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251103211119913.png" alt="image-20251103211119913" style="zoom:30%;" />

		 						3.被引用方法的功能要满足当前需求

	* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251103201613674.png" alt="image-20251103201613674" style="zoom:50%;" />

### 12.2方法引用的分类

#### 12.21引用静态方法:

* >格式:

	* 类名::静态方法

	* 范例: Integer::parseInt

		```java
		package Test;
		import java.util.ArrayList;
		import java.util.Collections;
		
		public class test {
		    public static void main(String[] args) {
		        ArrayList<String> list = new ArrayList<>();
		        Collections.addAll(list, "1", "2", "3", "4");
		        //parseInt方法是静态方法
		        list.stream().map(Integer::parseInt).forEach(System.out::println);
		    }
		}
		```

#### 12.22引用成员方法

* >引用其他类的成员方法

	* > 格式: 对象::成员方法

		* 其他类:其他类对象(new 对象名()——-创建其他类对象)::方法名
		* 本类:this::方法名(引用处不能是静态方法)
		* 父类:super::方法名(引用处不能是静态方法)



* >引用本类的成员方法

* >引用父类的成员方法

#### 12.23引用构造方法:

* > 格式:

	* 类名::new

	* 范例:Student::new

	* ```java
		package Test;
		
		import java.util.ArrayList;
		import java.util.Collections;
		
		public class test {
		    public static void main(String[] args) {
		        ArrayList<String> list = new ArrayList<>();
		        Collections.addAll(list, "zhangsan-23", "lisi-24", "wangwu-25");
		        list.stream().map(Student::new).forEach(System.out::println);
		
		
		    }
		}
		class Student{
		    private String name;
		    private int age;
		    public Student(String name,int age){
		        this.name=name;
		        this.age=age;
		    }
		    public Student(){
		
		    }
		
		    //为了和map匿名内部类里面的apply(String s)形参保持一致
		    public Student(String s){
		        String[] sp=s.split("-");
		        this.name=sp[0];
		        this.age=Integer.parseInt(sp[1]);
		    }
		    public String getName() {
		        return name;
		    }
		
		    public void setName(String name) {
		        this.name = name;
		    }
		
		    public int getAge() {
		        return age;
		    }
		
		    public void setAge(int age) {
		        this.age = age;
		    }
		    @Override
		    public String toString() {
		        return "Student{" +
		                "name='" + name + '\'' +
		                ", age=" + age +
		                '}';
		    }
		}
		```

#### 12.24:其他调用方式:

* >使用类名引用成员方法

	* >格式:

		* 类名::成员方法
		* 范例:String::substring

	* > 方法引用规则:

		* ```java
			package Test;
			
			import java.util.ArrayList;
			import java.util.Collections;
			import java.util.function.Function;
			
			public class test {
			    public static void main(String[] args) {
			        ArrayList<String> list = new ArrayList<>();
			        Collections.addAll(list, "zhangsan", "lisi", "w");
			        //变成大写后输出toUpperCase()是String类中的方法, 而且是无参的
			
			        list.stream().map(String::toUpperCase).forEach(System.out::println);
			        list.stream().map(new Function<String, String>() {
			            @Override
			            public String apply(String s) {
			                return s.toUpperCase();
			            }
			        }).forEach(System.out::println);
			        /*方法引用的规则(这种方式独有的):
			        * 1.需要有函数式接口
			        * 2.被引用的方法必须已经存在
			        * 3.被引用方法的形参, 需要跟抽象方法的第二个形参到最后一个形参保持一致, 返回值需要保持一致
			        * 4.被引用方法的功能需要满足当前的需求
			        *
			        * 抽象方法形参详解:
			        * 第一个形参: 表示被引用方法的调用者, 决定了可以引用哪些类中的方法
			        *            在Stream流中, 第一个参数一般都表示流里面的每一个数据
			        *            假设流里面的数据是字符串, 那么使用这种方式进行方法的引用, 只能引用String这个类中的方法
			        * 第二个形参到最后一个形参: 表示被引用方法的参数, 跟被引用的方法的参数保持一致, 如果没有第二个参数, 就表示被引用的方法是无参的
			        *
			        *局限性:不能引用所有类中的成员方法
			        *      是跟抽象方法的第一个形参保持一致的, 这个参数是什么类型, 就只能引用这个类型中的方法
			        * */
			    }
			}
			```

* >引用数组的构造方法

	* >格式:

		* 数据类型[]::new
		* 范例: int[]::
		
		* 
		
		* ```java
			package Test;
			import java.util.ArrayList;
			import java.util.Arrays;
			
			public class test {
			    public static void main(String[] args) {
			        ArrayList<Student> list = new ArrayList<>();
			        list.add(new Student("zhangsan", 12));
			        list.add(new Student("lisi", 13));
			        list.add(new Student("wangwu", 14));
			       /* String[] str = list.stream().map(new Function<Student, String>() {
			            @Override
			            public String apply(Student student) {
			                return student.getName();
			            }
			        }).toArray(String[]::new);*/
			        String[] str = list.stream().map(Student::toString).toArray(String[]::new);
			        System.out.println(Arrays.toString(str));
			    }
			}
			class Student {
			    private String name;
			    private int age;
			    public Student(String name, int age) {
			        this.name = name;
			        this.age = age;
			    }
			
			    public Student(String name){
			        this.name = name.split(",")[0];
			        this.age = Integer.parseInt(name.split(",")[1]);
			    }
			    public String getName() {
			        return name;
			    }
			
			    public void setName(String name) {
			        this.name = name;
			    }
			
			    public int getAge() {
			        return age;
			    }
			
			    public void setAge(int age) {
			        this.age = age;
			    }
			    @Override
			    public String toString() {
			        return this.name + "," + this.age;
			    }
			}
			```

## 13.异常和file:

### 13.1异常体系:

* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251104230716836.png" alt="image-20251104230716836" style="zoom: 33%;" />

* 异常体系最上层父类是Exception, 异常分为编译时异常和运行时异常
* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251104231726199.png" alt="image-20251104231726199" style="zoom: 25%;" />
* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251104231010358.png" alt="image-20251104231010358" style="zoom:25%;" />

```java
package Test;
import java.text.ParseException;
import java.text.SimpleDateFormat;
import java.util.Date;

public class test {
    public static void main(String[] args) throws ParseException {
        //编译时期异常(在编译阶段, 必须要手动处理, 否则代码报错)
        String time = "2023年1月1日";
        SimpleDateFormat sdf = new SimpleDateFormat("yyyy-MM-dd");
        Date date = sdf.parse(time);//必须要加上throws ParseException否则编译时会一直报错
        System.out.println(date);
        //运行时异常
        int[] arr = {1, 2, 3};
        System.out.println(arr[343]);
    }
}
```

* >异常的处理方式:

	* JVM默认的处理方式

		* 把异常名称,原因,及出现的位置输出在控制台
		* 程序停止执行, 下面的代码不会再执行了

	* 自己处理(捕获异常)

		* 目的:当代码出现异常时, 可以让程序继续往下执行

		* 常见问题:如果try中遇到了问题, 那么try下面的其他代码不会执行, 直接跳转到对应的catch, 如果没有对应的catch与之匹配, 则交给虚拟机处理

		* ```java
			package Test;
			
			public class test {
			    public static void main(String[] args){
			        int[] arr = {1, 2, 3};
			        try{
			            System.out.println(arr[343]);//此处出现了异常, 程序就会在这里创建一个ArrayIndexOutOfBoundsException对象
			                                         //new ArrayIndexOutOfBoundsException();
			                                         //拿着这个对象到catch的小括号中对比, 看括号中的变量是否可以接收这个对象, 能接收执行catch里面的代码
			        }catch(ArrayIndexOutOfBoundsException e){
			            System.out.println("索引越界异常");
			        }
			        System.out.println("看看我执行了吗");
			    }
			}
			```

		* 常见方法:

			* Throwable的成员方法

			* 

			* ```java
				package Test;
				
				public class test {
				    public static void main(String[] args){
				        int[] arr = {1, 2, 3};
				        try{
				            System.out.println(arr[343]);
				        }catch(ArrayIndexOutOfBoundsException e){
				            //toString()是返回异常的类型和异常的详细信息
				            String s = e.toString();
				            System.out.println(s);//java.lang.ArrayIndexOutOfBoundsException: Index 343 out of bounds for length 3
				            //getMessage()是返回异常的详细信息
				            System.out.println(e.getMessage());//Index 343 out of bounds for length 3
				            //printStackTrace()是打印异常的栈轨迹,错误信息输出在控制台
				            //                并且程序继续执行
				            e.printStackTrace();
				        }
				        System.out.println("看看我执行了吗");
				        System.err.println("aaa");//红色字体
				    }
				}
				```

	* 抛出异常

		* >throw和throws(编译时异常写)

​				       <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251105210909661.png" alt="image-20251105210909661" style="zoom: 33%;" />			

​					自定义异常:

```java
package Test;
import java.util.Scanner;
public class test {
    public static void main(String[] args) {
        girlFriend gf = new girlFriend();
        Scanner sc = new Scanner(System.in);
        while (true) {
            try {
                System.out.println("请输入姓名:");
                String name = sc.nextLine();
                gf.setName(name);

                System.out.println("请输入年龄:");
                String a = sc.nextLine();
                int age = Integer.parseInt(a);
                
                gf.setAge(age);
                break;
            }//转换为int类型
            catch (NumberFormatException e) {
                System.out.println("年龄格式有错误, 请输入数字");
            } catch (NameException e) {
                System.out.println("姓名或年龄输入错误");
            } catch (AgeException e) {
                System.out.println("年龄输入错误");
            }
        }
        System.out.println(gf);

    }
}
class girlFriend{
    private String name;
    private int age;
    public girlFriend() {
    }
    public girlFriend(String name, int age) {
        this.name = name;
        this.age = age;
    }
    public String getName() {
        return name;
    }
    public void setName(String name) {
        if(name.length()<3||name.length()>10){
            throw new NameException();
        }
        this.name = name;
    }
    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        if(age<0||age>50){
            throw new AgeException();
        }
        this.age = age;
    }
    @Override
    public String toString() {
        return "girlFriend{" +
                "name='" + name + '\'' +
                ", age=" + age +
                '}';
    }
}

class NameException extends RuntimeException{
    public NameException() {
    }
    public NameException(String message) {
        super(message);
    }
}
class AgeException extends RuntimeException{
    public AgeException() {
    }
    public AgeException(String message) {
        super(message);
    }
}
```

### 13.2File:

* > File的概述和构造方法

	* File对象就表示一个路径, 可以是文件路径, 也可以是文件夹路径

	* 这个路径可以是存在的, 也可以是不存在的

	* 绝对路径是带盘符的, 相对路径是不带盘符, 默认到当前项目下去找

	* file构造方法

		* 

		* ```java
			package Test;
			import java.io.File;
			public class test {
			    public static void main(String[] args) {
			        //1使用File(String pathname)构造方法创建文件对象
			        File file = new File("D:/develop/idea/code/basic-code/Test/src/Test/test.java");
			        //2使用File(File parent, String child)构造方法创建文件对象
			        File file2 = new File(file,"test2.java");
			        //3.使用File(String parent, String child)构造方法创建文件对象
			        File file3 = new File("D:/develop/idea/code/basic-code/Test/src/Test","test3.java");
			        System.out.println(file);
			        System.out.println(file2);
			        System.out.println(file3);
			    }
			}
			```

* >File的成员方法

  * 获取和判断

  * ```java
    package Test;
    import java.io.File;
    import java.text.SimpleDateFormat;
    import java.util.Date;
    public class test {
        public static void main(String[] args){
            //1.getAbsolutePath()返回定义文件时使用的路径
            File f1 = new File("basic-code/aaa");
            System.out.println(f1.getAbsolutePath());//D:\develop\idea\code\basic-code\basic-code\aaa
            //2.length()返回文件的长度
            System.out.println(f1.length());//0
            //3.getName()返回文件的名称
            System.out.println(f1.getName());//aaa
            //4.lastModified()返回文件的最后修改时间
            System.out.println(f1.lastModified());
            //将时间转换成yyyy-MM-dd HH:mm:ss格式
            SimpleDateFormat sdf = new SimpleDateFormat("yyyy-MM-dd HH:mm:ss");
            System.out.println(sdf.format(new Date(f1.lastModified())));
            //5.isDirectory()返回文件是否是目录
            System.out.println(f1.isDirectory());//false
            //6.isFile()返回文件是否是文件
            System.out.println(f1.isFile());
    
        }
    }
    ```

  * 创建, 删除mkdir(), mkdirs(), delete(), createNewFile()
  * ![image-20251106144112434](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251106144112434.png)

  * <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251106144142341.png" alt="image-20251106144142341" style="zoom: 50%;" />

  * 获取并遍历:listFile()

  * ```java
  	package Test;
  	import java.io.File;
  	public class test {
  	    public static void main(String[] args) {
  	        File f = new File("D:\\develop");
  	        //listFile方法
  	        File[] files  = f.listFiles();
  	        for (File file : files) {
  	            System.out.println(file);
  	        }
  	    }
  	}//1.调用File表示的路径不存在或者是文件, 或者要权限才能访问(如C盘)->null
  	 //2.空文件夹->长度是0的数组
  	 //3.有内容(包括隐藏文件)将所有文件文件夹的路径放在File数组中返回
  	```

  * ```java
  	package Test;
  	import java.io.File;
  	import java.io.FileFilter;
  	public class test {
  	    public static void main(String[] args) {
  	        File f = new File("D:\\develop");
  	        //listFile方法
  	        File[] arr = f.listFiles(new FileFilter() {
  	            @Override
  	            public boolean accept(File pathname) {
  	                return pathname.isFile()&&pathname.getName().endsWith(".txt");
  	            }
  	        });
  	    }
  	}
  	```

  * 练习

  * 递归

  * ```java
  	package Test;
  	import java.io.File;
  	import java.io.IOException;
  	public class test {
  	    public static void main(String[] args) throws IOException {
  	        File src = new File("C:\\");
  	        findAVI(src);
  	    }
  	    //用递归找出src目录下所有的avi文件
  	    public static void findAVI(File src){
  	        File[] files = src.listFiles();
  	        if(files==null){
  	            return;
  	        }
  	        for (File file : files) {
  	            if(file.isFile()){
  	                String name = file.getName();
  	                if(name.endsWith(".avi")){
  	                    System.out.println(file);
  	                }
  	            }else{
  	                findAVI(file);//文件夹递归
  	            }
  	        }
  	    }
  	}
  	```

  * 遍历文件夹中所有的文件种类和数目

  * ```java
  	package Test;
  	import java.io.File;
  	import java.io.IOException;
  	import java.util.HashMap;
  	import java.util.Map;
  	
  	public class test {
  	    public static void main(String[] args) throws IOException {
  	        File file = new File("D:\\develop\\");
  	        HashMap<String,Integer> map = getCount(file);
  	        System.out.println(map);
  	    }
  	    public static HashMap<String,Integer> getCount(File src){
  	        HashMap<String,Integer> map = new HashMap<>();
  	        File[] files = src.listFiles();
  	        if (files==null){
  	            return map;
  	        }
  	        for (File file : files) {
  	            if(file.isFile()){
  	                String[] name = file.getName().split("\\.");
  	                String end = name[name.length-1];
  	                if(map.containsKey(end)){
  	                    map.put(end, map.get(end)+1);
  	                }else{
  	                    map.put(end,1);
  	                }
  	            }else if(file.isDirectory()){
  	                HashMap<String, Integer> temp = getCount(file);
  	                for (Map.Entry<String, Integer> entry : temp.entrySet()) {
  	                    if(map.containsKey(entry.getKey())){
  	                        map.put(entry.getKey(),map.get(entry.getKey())+entry.getValue());
  	                    }else{
  	                        map.put(entry.getKey(), entry.getValue());
  	                    }
  	                }
  	            }
  	        }
  	        return map;
  	    }
  	}
  	```

  * ```java
  	public void deleteAll(File src){
  	    File[] files = src.listFiles();
  	    if (files==null){
  	        return;
  	    }
  	    for (File file : files) {
  	        if(file.isDirectory()){
  	            deleteAll(file);
  	        }else{
  	            file.delete();
  	        }
  	    }
  	    //最后把src空目录也删除了
  	    src.delete();
  	}
  	```

## 14.IO流:

### 14.1: IO流概述和体系

* >定义:

  * 用于读写文件中的数据(可以读写文件, 或网络中的数据…)
  * I:  Input      , O:  Output    , 流:像水流一样传输数据
  * IO流中, 是以程序为参照物进行读写, 是程序在读取文件中的数据, 是程序在往文件当中写出数据, (说成内存也可以, 因为程序就是运行在内存当中的)

* >分类:

  * 按照流的方向:分为   输入流(读取, 程序->文件)  和输出流(写出,  文件->程序)
  * 按照操作文件类型:分为   字节流(可以操作所有类型文件)  和 字符流(只能操作纯文本文件)
  	* 纯文本文件: Windows自带的记事本打开能读懂txt, md, xml, lrc……..

* >体系:

  * <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251106190235344.png" alt="image-20251106190235344" style="zoom: 25%;" />

  ### 14.2字节流:

  * OutputStream

  * 中的FileOutputStream

  * 写数据3种方式:write(int b)/(byte[] b)/(byte[] b, int off, int len)

  * ```java
    package Test;
    import java.io.FileOutputStream;
    import java.io.IOException;
    public class test {
        public static void main(String[] args) throws IOException {
            //1.创建文件输出流对象
            //参数是字符串的路径或者File对象都是可以的, 如果不存在创建一个, 已存在清空
            FileOutputStream fos = new FileOutputStream("Test\\aaa\\a.txt");
            //2.调用write方法写入数据, 写入97对应的字符a
            fos.write(97);
            //3.释放资源(如果不释放, 程序一直运行, 无法操作文件)
            fos.close();
        }
    }
    ```

  * 续写和换行

  * ```java
    package Test;
    import java.io.FileOutputStream;
    import java.io.IOException;
    public class test {
        public static void main(String[] args) throws IOException {
            FileOutputStream fos = new FileOutputStream("Test\\aaa\\a.txt", true);//续写文件
            String str = "aaaa";
            fos.write(str.getBytes());
            //换行
            //fos.write("\r\n".getBytes());
            //str = "bbbb";
            //fos.write(str.getBytes());
            fos.close();
        }
    }
    ```

  * InputStream

  * 中的FileInputStream->读取方法read()

  * ```java
    package Test;
    import java.io.FileInputStream;
    import java.io.IOException;
    public class test {
        public static void main(String[] args) throws IOException {
            FileInputStream fis = new FileInputStream("Test\\aaa\\a.txt");
            //循环读取
            int b;
            while((b = fis.read())!=-1){
                System.out.print((char)b);
            }
            /*错误的读取方式
            while(fis.read()!=-1){
                System.out.print((char)fis.read());
            }
            因为每read()一次，指针就会向后移动一位，所以每次读取的都是下一个字符
            * */
        }
    }
    ```

  * 拷贝文件

  * ```java
    package Test;
    import java.io.FileInputStream;
    import java.io.FileOutputStream;
    import java.io.IOException;
    public class test {
        public static void main(String[] args) throws IOException {
            FileInputStream fis = new FileInputStream("Test\\aaa\\a.txt");
            FileOutputStream fos = new FileOutputStream("Test\\aaa\\b.txt");
            int b;
            while((b = fis.read())!=-1){
                fos.write(b);
            }
            fos.close();
            fis.close();//先打开的输入流最后关
        }
    }
    ```

  * ```java
    package Test;
    import java.io.File;
    import java.io.FileInputStream;
    import java.io.FileOutputStream;
    import java.io.IOException;
    public class test {
        public static void main(String[] args) throws IOException {
            FileInputStream fis = new FileInputStream(new File("Test\\aaa\\a.txt"));
            FileOutputStream fos = new FileOutputStream(new File("Test\\aaa\\b.txt"));
            //改进拷贝速度
            byte[] bytes = new byte[1024*1024*5];//一次拷贝是5MB
            int b = 0;
            while((b = fis.read(bytes))!=-1){
                fos.write(bytes, 0, b);//不写成write(bytes)是为了避免最后重复读到残留的字节
            }
            fos.close();
            fis.close();
        }
    }
    ```

  * try…catch捕获异常

  * <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251107145459684.png" alt="image-20251107145459684" style="zoom: 50%;" />

  * 基本做法(finally中的代码块不论是否抛出异常都会执行)

  * ```java
  	package Test;
  	import java.io.File;
  	import java.io.FileInputStream;
  	import java.io.FileOutputStream;
  	import java.io.IOException;
  	public class test {
  	    public static void main(String[] args) {
  	        FileInputStream fis = null;
  	        FileOutputStream fos = null;
  	        try {
  	            fis = new FileInputStream(new File("Test\\aaa\\a.txt"));
  	            fos = new FileOutputStream(new File("Test\\aaa\\b.txt"));
  	            //改进拷贝速度
  	            byte[] bytes = new byte[1024*1024*5];
  	            int b = 0;
  	            while((b = fis.read(bytes))!=-1){
  	                fos.write(bytes, 0, b);//不写成write(bytes)是为了最后重复读到残留的字节
  	            }
  	        } catch (IOException e) {
  	            throw new RuntimeException(e);
  	        } finally {//!!!!!!finally块中的代码无论是否抛出异常都会执行!!!!
  	            if (fos != null) {//判断null是为了避免空指针异常
  	                try {
  	                    fos.close();
  	                } catch (IOException e) {//关闭流时也可能会抛出异常
  	                    throw new RuntimeException(e);
  	                }
  	            }
  	            if (fis != null) {
  	                try {
  	                    fis.close();
  	                } catch (IOException e) {
  	                    throw new RuntimeException(e);
  	                }
  	            }
  	        }
  	    }
  	}
  	```

### 14.3:字符集:

* >ASCII字符集(也叫做ASCII编码表):存储英文, 一个字节就足以

	<img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251107165028237.png" alt="image-20251107165028237" style="zoom:50%;" />

	* 计算机在存储英文的时候只需要一个英文就可以了:      0~127一共是128个字符, 而一个字节最多能表示256个字符
	* ![image-20251107165333504](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251107165333504.png)

* >GBK字符集:

	* ![image-20251107170937047](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251107170937047.png)
	* 规则1:  一个汉字使用两个字节进行存储:  一个字节最多存储2^8即256个字符, 而两个字节可以存储2^16即65535个字符, (太多字节浪费空间), 前面的第一个字节叫做高位字节
	* 规则2:  高位字节二进制一定以1开头(是为了和英文区分开来), 转成十进制之后是一个负数

* >Unicode字符集: 万国码

	* Unicode相关的编码规则

		* UTF-16 编码规则: 用2~4个字节保存

		* UTF-32编码规则: 固定使用四个字节保存

		* UTF-8编码规则: 用1~4个字节进行保存: 

			* ASCII用1个字节, 简体中文用3个字节
			* ![image-20251107172128219](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251107172128219.png)

			* <img src="C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251107172206457.png" alt="image-20251107172206457" style="zoom:200%;" />

* >乱码:

	* 产生原因:

		* 读取数据时未读完整个汉字![image-20251107200108948](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251107200108948.png)

		* 编码和解码的方式不统一:
			![image-20251107200207234](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251107200207234.png)

	* 解决方法:
		* 不要用字节流去读取文本文件
		* 编码解码时使用同一个码表, 同一个编码方式

* > 编码和解码

```java
package Test;
import java.io.UnsupportedEncodingException;
import java.util.Arrays;
public class test {
    public static void main(String[] args) throws UnsupportedEncodingException {
        //编码和解码的代码实现方式
        String string0 = "ai你哟";
        byte[] bytes1 = string0.getBytes();
        System.out.println(Arrays.toString(bytes1));//[97, 105, -28, -67, -96, -27, -109, -97]
        //解码
        String string = new String(bytes1);
        System.out.println(string);
        
        byte[] bytes2 =  string.getBytes("GBK");
        System.out.println(Arrays.toString(bytes2));//[97, 105, -60, -29, -45, -76]
        System.out.println(new String(bytes2,"GBK"));
    }
}
```

### 14.4:字符流:

* > 概述:

	* =字节流+字符集,,底层就是字节流
	* ![image-20251107203905697](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251107203905697.png)
	* 特点:
		*  输入流: 一次读一个字节, 遇到中文时, 一次读多个字节
		* 输出流: 底层会把数据按照指定的编码方式进行编码, 变成字节再写到文件中

* > 使用场景: 

	* 对于一些纯文本文件进行读写操作
	* 为了解决乱码问题

* > FileReader和FileWriter的代码实现:

	* FileReader: 

	  * 创建字符输入流对象->构造方法: public FileReader(File file);;public FileReader(String pathname)——如果文件不存在直接报错

	  * 读取数据->成员方法: public int read();

	  	​								  public int read(char[] buffer)—–读取多个数据, 读到末尾返回-1

	  	* 细节: 按字节进行读取, 遇到中文, 一次读取多个字节, 读取后解码, 返回一个整数;;读到文件末尾了, read方法返回-1
	
	  * 释放资源close()
	
	* FileWriter:
	
		* ![image-20251108122451859](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251108122451859.png)
	
	* 代码:
	
	* ```java
		package Test;
		import java.io.FileReader;
		import java.io.FileWriter;
		import java.io.IOException;
		public class test {
		    public static void main(String[] args) throws IOException {
		        FileReader fr = new FileReader("Test\\aaa\\a.txt");
		        //读取数据
		        int ch;
		        while ((ch = fr.read()) != -1) {
		            System.out.print((char) ch);//ch表示读取到的字符的编码值
		        }
		        //read()方法
		        //1.默认也是一个字节一个字节的读取, 如果遇到中文就会一次读取多个
		        //2.读取之后, 方法的底层还会进行解码并转成十进制(字符集上的编码值)
		        //  最终把这个十进制作为返回值
		        FileReader fr2 = new FileReader("Test\\aaa\\a.txt");
		        //有参的read()方法:read(chars): 读取数据, 解码, 强转三步合并了, 把强转之后的字符放到数组当中
		        //=空参的read()+强转+解码
		        char[] arr = new char[2];
		        int len;
		        while((len = fr2.read(arr))!=-1){
		            System.out.println(new String(arr, 0, len));//实际读了多少个就转多少个
		        }
		        fr.close();
		        fr2.close();
		        //FileWriter的相关方法
		        FileWriter fw = new FileWriter("Test\\aaa\\a.txt");
		        fw.write("hello world");
		        String str = "hello world";
		        char[] arr2 = str.toCharArray();
		        fw.write(arr2);
		        fw.write(arr2, 0, arr2.length);//从数组的第0个位置开始写, 写arr2.length个
		        fw.write("hello world", 0, "hello world".length());
		        fw.close();
		    }
		}
		```

* >字符流原理解析

	* 缓冲区: 长度为8192的字节数组, 目的是提高效率
	* 读取: ![image-20251108123824281](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251108123824281.png)

	* 写到目的文件:
		![image-20251108124606520](C:/Users/ZY/AppData/Roaming/Typora/typora-user-images/image-20251108124606520.png)

* > 综合练习

	* ```java
		package Test;
		
		import java.io.File;
		import java.io.FileInputStream;
		import java.io.FileOutputStream;
		import java.io.IOException;
		public class test {
		    public static void main(String[] args) throws IOException {
		        //拷贝一个文件夹, 考虑子文件夹
		        //创键文件夹, 以及要拷贝的地方
		        File src = new File("D:\\typora笔记");
		        File dest = new File("D:\\develop");
		        //开始调用方法进行拷贝
		        copydir(src, dest);
		    }
		    private static void copydir(File src, File dest) throws IOException {
		        //新建目标文件夹
		        dest.mkdirs();
		        //获取当前文件夹下的所有文件
		        File[] files=src.listFiles();
		        for (File file : files) {
		            //判断是否是文件
		            if(file.isFile()){
		                //是文件直接拷贝
		                //创建读和写的流
		                FileInputStream fis = new FileInputStream(file);
		                FileOutputStream fos = new FileOutputStream(new File(dest, file.getName()));//创建一个新的文件, 名字和源文件一致
		                //拷贝文件
		                int len;
		                //创建一个数组来提高读取的速度
		                byte[] bytes = new byte[1024];
		                while((len = fis.read(bytes))!=-1){
		                    //将读取到的内容写入到目标文件当中
		                    fos.write(bytes,0,len);
		                }
		                //及时关闭流
		                fos.close();
		                fis.close();
		            }else{
		                copydir(file, new File(dest, file.getName()));
		            }
		        }
		    }
		}
		```

### 14.5缓冲流,转换流,打印流(字节,字符)

#### 一.缓冲流

* > 概览:缓冲流自带长度为8192的缓冲区

	* ![image-20251108151833371](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20251108151833371.png)

* > 字节缓冲流: 

	* 相关方法:

		* public BufferedInputStream(InputStream is): 把基本流包装成高级流, 提高读取数据的性能(原理是底层自带了长度是8192的缓冲区提高性能)

		* publuc BufferedOutputStream(OutputStream os): 把基本流包装成高级流, 提高写出数据的性能.

		* ```java
			package Test;
			import java.io.*;
			public class test {
			    public static void main(String[] args) throws IOException {
			        BufferedInputStream bis = new BufferedInputStream(new FileInputStream("Test\\aaa\\a.txt"));
			        BufferedOutputStream bos = new BufferedOutputStream(new FileOutputStream("Test\\aaa\\b.txt"));
			        int len = 0;
			        while((len = bis.read()) != -1){
			            bos.write(len);
			        }
			        bis.close();
			        bos.close();
			    }
			}
			```

	* 字节缓存流的读写原理
		* ![image-20251108191439035](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20251108191439035.png)

* > 字符缓冲流:

	* 相关方法:
		* public BufferedReader(Reader r)//BufferedWriter(Writer r):基本流变高级流(原理是底层自带了长度为8192的缓冲区提高性能)
		* 字符缓冲输入流:public String readLine():读取一行数据, 如果没有数据可读了, 会返回null
		* 字符缓冲输出流:public void newLine():*跨平台的换行*Mac: \r , , windows: \r\n,, Linux: \n
	* 注意点: 
		* 缓冲流自带长度为8192的缓冲区
		* 字节缓冲流缓冲区是byte类型的长度是8k, 字符缓冲流缓冲区是char类型的长度是16k
		* 字节缓冲流提升的效率明显, 字符缓冲流提升不明显,因为字符流的基本流当中已经有缓冲区了, 主要是两个特有方法

* > 综合练习

	* 

	* ```java
		package Test;
		import java.io.*;
		import java.util.*;
		public class test {
		    public static void main(String[] args) throws IOException {
		        /*//拷贝文件的四种方式
		        long start = System.currentTimeMillis();
		        //method1();//585ms
		        //method2();//3ms
		        //method3();//10ms
		        //method4();//1ms
		        long end = System.currentTimeMillis();
		        System.out.println("耗时：" + (end - start) + "毫秒");*/
		        //recover2();
		        count();
		    }
		    private static void method1() throws IOException {
		        //字节的基本流:一次读写一个字节
		        FileInputStream fis = new FileInputStream("Test\\aaa\\a.txt");
		        FileOutputStream fos = new FileOutputStream("Test\\aaa\\b.txt");
		        int len = 0;
		        while((len = fis.read())!=-1){
		            fos.write(len);
		        }
		        fis.close();
		        fos.close();
		    }
		    private static void method2() throws IOException {
		        //字节基本流, 一次读取一个数组
		        FileInputStream fis = new FileInputStream("Test\\aaa\\a.txt");
		        FileOutputStream fos = new FileOutputStream("Test\\aaa\\b.txt");
		        int len = 0;
		        byte[] bytes = new byte[8192];
		        while((len = fis.read(bytes))!=-1){
		            fos.write(bytes, 0, len);
		        }
		        fis.close();
		        fos.close();
		    }
		    private static void method3() throws IOException {
		        //字节缓冲流
		        BufferedInputStream bis = new BufferedInputStream(new FileInputStream("Test\\aaa\\a.txt"));
		        BufferedOutputStream bos = new BufferedOutputStream(new FileOutputStream("Test\\aaa\\b.txt"));
		        int len = 0;
		        while((len = bis.read())!=-1){
		            bos.write(len);
		        }
		        bis.close();
		        bos.close();
		    }
		    private static void method4() throws IOException {
		        //字节缓冲流一次读写一个数组
		        BufferedInputStream bis = new BufferedInputStream(new FileInputStream("Test\\aaa\\a.txt"));
		        BufferedOutputStream bos = new BufferedOutputStream(new FileOutputStream("Test\\aaa\\b.txt"));
		        int len = 0;
		        byte[] bytes = new byte[8192];
		        while((len = bis.read(bytes))!=-1){
		            bos.write(bytes, 0, len);
		        }
		        bis.close();
		        bos.close();
		    }
		    private static void recover1() throws IOException {
		        //将a.txt文件恢复到一个新文件中
		        BufferedReader br = new BufferedReader(new FileReader("Test\\aaa\\a.txt"));
		        BufferedWriter bw = new BufferedWriter(new FileWriter("Test\\aaa\\b.txt"));
		        //先读取
		        ArrayList<String> list = new ArrayList<>();
		        //调用readLine()方法
		        String line;
		        while((line = br.readLine())!=null){
		            list.add(line);
		        }
		        Collections.sort(list, new Comparator<String>() {
		            @Override
		            public int compare(String o1, String o2) {
		                int num1 = Integer.parseInt(o1.split("\\.")[0]);
		                int num2 = Integer.parseInt(o2.split("\\.")[0]);
		                return num1-num2;
		            }
		        });
		        //将list中所有的元素写在新文件中
		        for (String string : list) {
		            bw.write(string);
		            bw.newLine();//newLine()表示换行
		        }
		        br.close();
		        bw.close();
		    }
		    private static void recover2() throws IOException {
		        //利用treemap进行操作
		        //把元素添加到treemap当中就会自动的排序了
		        BufferedReader br = new BufferedReader(new FileReader("Test\\aaa\\a.txt"));
		        BufferedWriter bw = new BufferedWriter(new FileWriter("Test\\aaa\\b.txt"));
		        //先读取
		        //调用readLine()方法
		        TreeMap<Integer, String> map = new TreeMap<>();
		        String line;
		        while((line = br.readLine())!=null){
		            String[] arr = line.split("\\.");//split的作用是把字符串变成字符数组, 两个\是避免和正则表达式中的.而转义的
		            map.put(Integer.parseInt(arr[0]), line);//写成arr[1]就没有序号了
		
		        }
		        //将map写到文件中
		        Set<Map.Entry<Integer, String>> entries = map.entrySet();
		        for (Map.Entry<Integer, String> entry : entries) {
		            bw.write(entry.getValue());
		            bw.newLine();
		        }
		        br.close();
		        bw.close();
		    }
		    private static void count() throws IOException {
		        //获取count
		        BufferedReader br = new BufferedReader(new FileReader("Test\\aaa\\a.txt"));
		        int count = Integer.parseInt(br.readLine());
		        br.close();
		        //执行
		        if(count<=3){
		            System.out.println("欢迎使用本软件, 第"+count+"次使用免费~");
		        }else{
		            System.out.println("本软件只能免费使用3次, 欢迎您注册会员后继续使用~");
		        }
		        count++;
		        BufferedWriter bw = new BufferedWriter(new FileWriter("Test\\aaa\\a.txt"));//这一行不能放在上面, 否则每次运行就会清空a.txt使得int转换错误
		        //将count重新写入
		        //创建会覆盖原文件
		        bw.write(count+"");
		        bw.close();
		    }
		}
		```

#### 二.转换流:

* > 概述及原理

	* 是字符流和字节流之间的桥梁
	* <img src="C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20251108215400979.png" alt="image-20251108215400979" style="zoom:50%;" />

* > 代码实现

	* ```java
		package Test;
		import java.io.*;
		import java.nio.charset.Charset;
		public class test {
		    public static void main(String[] args) throws IOException {
		        //利用转换流按照指定字符编码读取
		        //1.jdk11以前
		       /* InputStreamReader isr = new InputStreamReader(new FileInputStream("D:\\develop\\idea\\code\\basic-code\\HelloWorld.txt"), "UTF-8");
		        int ch = 0;
		        while ((ch = isr.read()) != -1) {
		            System.out.print((char) ch);
		        }
		        isr.close();*/
		        //2.jdk11以后
		        FileReader fr = new FileReader("D:\\develop\\idea\\code\\basic-code\\HelloWorld.txt", Charset.forName("UTF-8"));
		        int ch = 0;
		        while ((ch = fr.read()) != -1) {
		            System.out.print((char) ch);
		        }
		        fr.close();
		        //3.利用转换流按照指定字符编码写出
		      /*  OutputStreamWriter osw = new OutputStreamWriter(new FileOutputStream("Test\\aaa\\a.txt"), "GBK");
		        osw.write("你好中国");
		        osw.close();*/
		        //
		        FileWriter fw = new FileWriter("Test\\aaa\\a.txt", Charset.forName("GBK"));
		        fw.write("你好中国");
		        fw.close();
		    }
		}
		```

	* 字节流转换字符流

	* ```java
		public class test {
		    public static void main(String[] args) throws IOException {
		        BufferedReader br = new BufferedReader(
		                new InputStreamReader(
		                new FileInputStream("D:\\develop\\idea\\code\\basic-code\\HelloWorld.txt")));
		        String str;
		        while((str = br.readLine())!=null){
		            System.out.println(str);
		        }
		    }
		}
		```

#### 三.序列化流和反序列化流Object:

* > 概览

	* <img src="C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20251109095934848.png" alt="image-20251109095934848" style="zoom:50%;" />

* > 序列化流/对象操作输出流:

	* 可以把java中的对象(new Student)写到本地文件中

	* 构造方法: public ObjectOutputStream(OutputStream out)把基本流包装成高级流

	* 成员方法: public final void writeObject(Object obj)把对象序列化(写出到文件当中)

* > 反序列化流/对象操作输入流

	* 可以把序列化到本地文件中的对象, 读取到程序中来
	* <img src="C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20251109103616346.png" alt="image-20251109103616346" style="zoom: 50%;" />

	* 版本号:

		* 理解<img src="C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20251109105740415.png" alt="image-20251109105740415" style="zoom: 50%;" />

		* 创建方式

			* 调整idea勾选选项<img src="C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20251109105958259.png" alt="image-20251109105958259" style="zoom:25%;" />

			* 悬停在类名, 显示添加

* <img src="C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20251109110902462.png" alt="image-20251109110902462" style="zoom:50%;" />

* > 代码实现

	* ```java
		package Test;
		import java.io.*;
		public class test {
		    public static void main(String[] args) throws IOException, ClassNotFoundException {
		        Student stu = new Student();
		        stu.setName("张三");
		        stu.setAge(18);
		        //创建序列化流的对象
		        ObjectOutputStream oos = new ObjectOutputStream(new FileOutputStream("Test\\aaa\\a.txt"));
		        oos.writeObject(stu);
		        oos.close();
		        ObjectInputStream ois = new ObjectInputStream(new FileInputStream("Test\\aaa\\a.txt"));
		        Student stu1 = (Student) ois.readObject();
		        System.out.println(stu1.toString());//name:张三,age:0
		        ois.close();
		    }
		}
		class Student implements Serializable {
		    @Serial
		    private static final long serialVersionUID = 5035801477520187138L;
		    private String name;
		    private transient int age;//transient关键字修饰的成员变量不会被序列化
		    public Student(String name,int age){
		        this.name=name;
		        this.age=age;
		    }
		    public Student() {
		    }
		    public String getName(){
		        return this.name;
		    }
		    public int getAge(){
		        return this.age;
		    }
		    public void setName(String name){
		        this.name=name;
		    }
		    public void setAge(int age){
		        this.age=age;
		
		    }
		    @Override
		    public String toString(){
		        return "name:"+this.name+",age:"+this.age;
		    }
		}
		```

#### 四.打印流:

* >  概览

	* ![image-20251109145044417](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20251109145044417.png)

	* 打印流只能写,所以只有输出流

* > 特点

	* 只操作文件目的地, 不操作数据源
	* *特有的写出方法*可以实现, 数据原样写出(打印97, 文件中就是97)

	* *特有的写出方法*, 可以实现自动刷新, 自动换行,
		* 打印一次数据 = 写出+换行+刷新

* > 分类

	* 一般是只PrintStream, PrintWriter两个类

	* 字节打印流:

		* 相关方法![image-20251109150027379](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20251109150027379.png)     ![image-20251109150246991](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20251109150246991.png)

		* ```java
			public class test {
			    public static void main(String[] args) throws FileNotFoundException, UnsupportedEncodingException {
			        PrintStream ps = new PrintStream(new FileOutputStream("Test\\aaa\\a.txt"), true, "UTF-8");
			        ps.println(97);
			        ps.printf("a=%d", 97);
			        ps.close();
			    }
			}
			```

	* 字符打印流:

		* 相关方法:![image-20251109150943663](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20251109150943663.png)		![image-20251109151028668](C:\Users\ZY\AppData\Roaming\Typora\typora-user-images\image-20251109151028668.png)

		* ```java
			public class test {
			    public static void main(String[] args) throws IOException {
			        PrintWriter pw = new PrintWriter(new FileWriter("Test\\aaa\\a.txt", true));
			        pw.println(97);
			        pw.printf("你好%d", 97);
			        pw.close();
			        //特殊的打印流, 系统中的标准输出流, 是不能关闭的, 在系统中是唯一的
			        PrintStream ps = System.out;//public static final PrintStream out = null;调用System类的静态方法out
			        ps.println("你好97");// 打印到控制台
			        ps.close();
			    }
			}
			```

#### 五.解压缩流:

* > 解压

	* 压缩包中的每一个文件都是ZipEntry形式
	* 解压本质: 把每一个ZipEnrty按照层级拷贝到本地另一个文件夹中

* > 代码实现

	* ```java
		public static void unzip(File src, File dest) throws IOException {
		    //将压缩包解压到目的地
		    //1.创建Zip
		    ZipInputStream zip = new ZipInputStream(new FileInputStream(src));//将src解压到dest
		    ZipEntry entry;//压缩包都是以ZipEntry的形式存在的
		    while((entry = zip.getNextEntry())!=null){
		        String name = entry.getName();
		        if(entry.isDirectory()){
		            //如果`是`文件夹就创建文件夹
		            File dir = new File(dest, name);
		            dir.mkdirs();
		            //这里不关闭是因为zip.closeEntry()会关闭zip流
		        }else{
		            FileOutputStream fos = new FileOutputStream(new File(dest, name));
		            int b = 0;
		            while((b = zip.read())!=-1){
		                fos.write(b);
		            }
		            fos.close();
		            zip.closeEntry();
		        }
		    }
		    zip.close();
		}
		```

	* 压缩变成空的了??

	* ```java
		public class test {
		    public static void main(String[] args) throws IOException {
		        File src = new File("D:\\develop\\TestFile\\aaa");
		        //1.创建压缩文件夹
		        File destParent = src.getParentFile();
		        File dest = new File(destParent, src.getName()+".zip");//父级目录+源文件名.zip,确保压缩包和源文件夹同名
		        //2.遍历src文件
		        ZipOutputStream zos = new ZipOutputStream(new FileOutputStream(dest));
		        toZip(src, zos, src.getName());
		        zos.close();
		      /*  //删除
		        File file = new File("D:\\develop\\TestFile\\aaa.zip");
		        file.delete();*/
		    }
		    public static void toZip(File src, ZipOutputStream zos, String name) throws IOException {
		        File[] files = src.listFiles();
		        for (File file : files) {
		            if(file.isFile()){
		                ZipEntry entry = new ZipEntry(name+"\\"+file.getName());//拼接压缩包中的路径
		                zos.putNextEntry(entry);
		                //将文件写入到压缩包
		                FileInputStream fis = new FileInputStream(file);
		                int b;
		                while((b = fis.read())!=-1){
		                    zos.write(b);
		                }
		                fis.close();
		                zos.closeEntry();//关闭当前目录是为了下一个目录的写入,因为单个文件读完就是读完了
		            }else{
		                toZip(file,zos, name+"\\"+file.getName());
		            }
		        }
		    }
		}
		```

### 14.6常用工具包:

* > Commons-io

	* 是apache开源基金组织提供的一组有关IO操作的开源工具包
	* 作用是提高IO流的开发效率

* > hutool

	* [hutool官网https://hutool.cn/](https://hutool.cn/)
	* 