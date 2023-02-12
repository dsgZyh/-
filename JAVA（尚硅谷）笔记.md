## JAVA

### 1.  JAVA 基础知识图解

![image-20230211190137514](C:\Users\aaa\AppData\Roaming\Typora\typora-user-images\image-20230211190137514.png)


### 1.1 JAVA语言的特点
#### 1.1.1 特点一 ： **面向对象**
	- 两个基本概念：类、对象
	- 三大特性：封装、继承、多态
#### 1.1.2 特点二：**健壮性**
	- 吸收了C/C++语言的优点、但去掉了其影响程序健壮性的部分(如指针、内存的申请与释放等)，提供了一个相对安全的内存管理和访问机制
#### 1.1.3 特点三：跨平台性
	- 跨平台性：通过JAVA语言编写的应用程序在不同的系统平台上都可以运行。“wrute once,run anywhere”
	- 原理：只要在需要运行JAVA应用的操作系统上，先安装一个JAVA虚拟机(JVM java Virtual Machine)即可，由JVM来负责JAVA程序在该系统中的运行

### 1.2 JAVA语言运行机制及运行过程

#### 1.2.1 **JAVA两种核心机制**
	- JAVA虚拟机（JAVA Virtal Machine）
	- 垃圾收集机制 （Garbage Collection）

#### 1.2.2 **java虚拟机**
	- jVM是一个虚拟机的计算机，具有指令集并使用不同的存储区域。复杂执行指令。管理书籍数据、内存、寄存器。
	- 对于不同平台，有不同的虚拟机。
	- 只有某平台提供了对应的java虚拟机，java程序才可以在此平台运行
	- java虚拟机机制屏蔽了底层运行平台的差别，实现了“一次编译，到处运行”
.java -> .class -> JVM 

#### 1.2.3 **垃圾回收**

	- 不再使用的内存空间应回收——垃圾回收
	- - C/C++等语言中，由程序员负责回收无用的内存
	- - JAVA语言消除了程序员回收无用内存空间的责任；它提供了一种系统线程跟踪存储空间的分配情况。并在JVM空闲时，检查并释放那些可被释放的存储空间。
	- 垃圾回收在JAVA程序运行过程中自动进行，程序员无法精确控制和干预。

#### 1.2.4 java环境搭建
	JDK (JAVA Development Kit JAVA开发工具包)
	JRE (JAVA Runtime Environment JAVA运行环境)
	- JDK = JRE + 开发工具集 （例如javac编译工具等）
	- JRE = JVM + java SE 标准类库
	JDK 官方地址：
		https://www.oracle.com
		java.sun.com


![image-20230211212950189](C:\Users\aaa\AppData\Roaming\Typora\typora-user-images\image-20230211212950189.png)

PATH ： windows命令在运行时搜寻的路径
​	

#### 1.2.5 JAVA运行过程
	步骤：
	1. 将java代码编写到扩展名为.java的文件中。
	2. 通过javac命令对java源文件进行编译
	3. 通过java命令对生成的class字节码文件运行

** JAVA严格区分大小写**

#### 1.2.6 JAVA注释
 	- 单行注释：//
 	- 多行注释：/**/
 	- 文档注释(Java特有)：
 	- - 格式：/**
 	- -      @author 指定java程序的作者
 	- - 	 @version 指定源文件
 	- - 	 */
 	- 注释内容可以被JDK提供的工具javadoc所解析，生成一套以网页文件形式体现的该程序的说明文件。