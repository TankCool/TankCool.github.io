---
layout: default
---

## 1.1 第一个java程序：Hello World

### 上课啦，准备好小板凳\*_*

新建一个文本文件，文件名为HelloWorld.java，然后输入以下代码
```java
public class HelloWorld {
  public static void main(String[] args) {
    // Prints "Hello, World" in the terminal window.
    System.out.println("Hello, World");
  }
}
```

打开命令行窗口，键入以下命令进行代码编译

	javac HelloWorld.java

如果没有报错的话，说明编译成功，接着就是键入执行命令

	java HelloWorld

以上就是一个基本的hello world了。

接着我们进行一个简单的扩展，在执行的时候传入参数，也就是往main函数的args里面传入信息，然后在控制台打印出来。

```java
public class BetterHelloWorld{
  public static void main(String[] args){
    System.out.print("I think ");
    //循环数组，打印每一项参数
    for (int i = 0; i < args.length ; i++) {
      System.out.print(args[i] + " ");
    }
    System.out.println();
  }
}
```

在命令行下编译并执行看结果

	javac BetterHelloWorld.java
	java BetterHelloWorld Joyce Chu is so kawayi.


### 实验时间到^_^

* HelloWorld.java 的代码改成以下这样，编译看会出现什么情况。

```java
public class MyHelloWorld {
  public static void main(String[] args) {
    // Prints "Hello, World" in the terminal window.
    System.out.println("Hello, World");
  }
}
```

* 接着我们把代码里面的public去掉，再编译看会出现什么情况。

```java
class MyHelloWorld {
  public static void main(String[] args) {
    // Prints "Hello, World" in the terminal window.
    System.out.println("Hello, World");
  }
}
```
在这里只需要记住，一个java文件只有一个public的类(可以有多个不是public修饰的类)，且名字必须和文件名一致。

### 小作业来啦$_$

1. 编写一个程序 TenTimeGoodGoodStudy.java，打印"好好学习，天天向上"10次！
2. 编写一个程序 BestHelloWorld.java，再传入三个人的名字，并倒序打印输出。例如输入

		java BestHelloWorld Justin Alice Tom

	应该输出

		Tom Alice Justin

	友情提示，记得参考上面给出的代码哦。
