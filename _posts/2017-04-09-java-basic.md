---
layout: default
---
### java基础知识
java是一门成熟且强大的语言，是程序员必不可少的重要技能之一。Java具有简单性、面向对象、分布式、健壮性、安全性、平台独立与可移植性、多线程、动态性等特点。Java可以编写桌面应用程序、Web应用程序、分布式系统和嵌入式系统应用程序等。下面记录一些java的基础知识，方便日后复习查阅。

#### 8种基础数据类型
	byte short int long float double boolean char
	
对应的引用类型

	Byte Short Integer Long Float Double Boolean Character	

#### 静态方法和实例方法的区别
* 静态方法不能使用this关键字，实例方法可以
* 调用静态方法不需要创建对象，而实例方法则需要先创建对象
* 静态方法只能访问静态成员，实例方法可以访问静态成员和实例成员

#### 不允许创建泛型数组
	Item[] item = new Item[n];//Error
	
应该这么处理

	Item[] item = (Item[]) new Object[n];//Warn but good to go

由于Java使用擦除(erasure)实现的泛型，在运行时无法知道确切的类型信息，因此不能创建相应类型的数组.

未完待续

2017-04-09 创建

[返回](../../../)
