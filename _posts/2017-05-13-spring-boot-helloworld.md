---
layout: default
---

### 什么是Spring Boot

[Spring Boot官网](http://projects.spring.io/spring-boot/)

简单地说就是Spring Boot可以让我们快速地创建独立的，产品级别的Spring应用。Spring Boot使用“习惯优于配置”的理念让我们可以很快地把项目运行起来，使用Spring Boot我们可以不用或者只需要很少的Spring配置。

### Spring Boot的优点

* 快速创建独立的Spring应用
* 内置Tomcat Jetty Undertow(无需部署war)
* 提供可选择的starter，简化你的Maven配置
* 尽可能地提供Spring自动配置
* 准生产级别的应用监控
* 无代码生成和xml配置

### 快速开始

本文使用的IDE是[Intellij Idea](https://www.jetbrains.com/idea/)

#### 创建项目

##### 打开Idea新建一个项目  

* 选中Spring Initializr，选择JDK版本，然后点击下一步  
![](https://tankcool.github.io/assets/images/spring-boot-helloworld/001.png)
* 修改包名、项目名称、项目描述，然后点击下一步
![](https://tankcool.github.io/assets/images/spring-boot-helloworld/002.png)
* 选择依赖，这里只需要勾选Web里面的Web，然后点击下一步
![](https://tankcool.github.io/assets/images/spring-boot-helloworld/003.png)
* 修改项目路径到你想要的位置
![](https://tankcool.github.io/assets/images/spring-boot-helloworld/004.png)

点击完成，项目就创建成功了。

#### 自定义Controller
新建一个简单的controller，仅仅是往页面返回一个字符串，因此用的是@RestController注解(方法名称随意)

```java
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;

@RestController
public class HelloWorldController {

    @RequestMapping("/hello")
    public String index(){
        return "Hello world. Welcome to learn spring boot!";
    }
}
	
```

运行项目，然后在浏览器访问[http://localhost:8080/hello](http://localhost:8080/hello)  
到目前为止，我们没写过一行配置，这就是Spring boot给我们带来的巨大好处，我们不需要做任何配置就可以把项目跑起来。
![](https://tankcool.github.io/assets/images/spring-boot-helloworld/005.png)

### 总结
使用Spring Boot可以非常快速搭建项目，我们不需要或者只需要很少的Spring配置就可以创建一个生产级别的项目，所以Spring Boot非常适用于构建微服务。 


2017-05-13 创建

[返回](../../../)	