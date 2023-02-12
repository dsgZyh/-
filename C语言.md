## C 语言

> 2023-02-8 17:41

### 1.数据类型
|数据类型|字节长度|
|---|---|
|int | 4B|
|float| 4B|
|double |8B|
|char | 1B|
|short int | 2B|
|long int | 8B|
|signed | 4B|
|unsigned | 4B|

### 2.存储关键字

1. register 
	register 是寄存器的意思，用register修饰的变量是寄存器变量
	定义的变量不一定真的放在寄存器里
	不能定义数组
	只能修饰整型的，不能修饰浮点型的
2. static 
	static是静态的意思
	static可以修饰全局变量、局部变量、函数
3. const
   	const是常量的意思
   	用const修饰的变量是只读的，不能修改它的值
   	```cont int a=101;//	在定义的时候 a 用了const修饰```
   	```a=1;//错误的```
	const可以修饰指针
4. extern 是外部的意思，一般用于函数和全局变量的声明。
> register(寄存器) static(静态) entern(外部)

### 控制语句
if else break for while do switch case goto default

### 其他关键字
1. sizeof
	用来测变量、数组的占用储存空间的字节
2. typedef
	用来重新给数据类型命名
3. volatile 意思是易改变的
	用volatile定义的变量，是易改变的，即告诉计算机用volatile修饰的变量的时候，重新去内存中取保证用的是最新的值，而不是寄存器中的备份



![image-20230209155008038](C:\Users\aaa\AppData\Roaming\Typora\typora-user-images\image-20230209155008038.png)
