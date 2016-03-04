# spring-boot

## 更新
> 便于查看是否有重要更新
- h819-commons : 1.0.10
- spring-boot-web : 0.1.0
- 逐步发布其他项目  ...

## 概述
做这个项目的想法来自于 [springside](https://github.com/springside/springside4/) ,           当时自己在不停的尝试各种框架和实现技术，为了选某一种实现而比来比去大费脑筋，
[springside](https://github.com/springside/springside4/)   给了一个很好的示范，从中学习到了很多知识，感叹是水太深了，什么时候能学完呢 --

Spring 现在基本上也一统江湖了，只要你想要的解决方案，Spring 基本上都有相关实现，没事可以多看看他的 [项目](http://spring.io/projects/)。

我的习惯是，一边学习一边敲代码，读书笔记就用注释写在代码示例里，我只记住我做过什么就可以了，当需要相关功能的时候，到示例里去找，扫一眼代码写法，读一下注释，基本上也就知道怎么编写了。

随着对相关原理理解的加深，代码不停的 Refactor，就算是自己的编程经验总结吧。

项目取名为 **spring-boot** ，意在显示的指出用的是 ==Spring Boot==。

h819 是我的 id。

这些项目会随着自己的总结，不停的添加和优化，示例也会越来越多。

## 项目简介


### spring-boot-web
> spring-boot-web

基于 Spring Boot 的 J2EE 开发实践，不发明什么，只是探索一种快速开发体验，开箱即用。

#### 核心组件
- spring boot

#### Data
- spring data JPA
- hibernate
- querydsl

#### Web
- spring mvc
- FreeMarker Template
- Bootstrap
- JQuery
- Ace Admin

#### security
- spring security
- spring security oauth2

#### Web Server
- tomcat
- jetty

#### DB Server
- mysql
- oracle

#### Environment
- Intellij IDEA
- git

#### Utils
- h819 commons
- Apache Commons
- Guava
- fastjson

---

### h819-commons
> h819-commons

这是一个基础工具包，能总结出来的都放在这里，可以生成 jar 文件引用到其他项目中，模拟 [apache commons](https://commons.apache.org/) 做法，做成一个符合自己需要的工具包。

可以多翻翻代码，里面有各种例子总结。

值得提的工具有：

#### java se commons

Components | Description | Source
---|---|---
Ftp | 可以连接 ftp 和 sftp | /commons
Exec  | java 执行系统命令 | /commons
Pdf  | Pdf 新建、加密解密、加水印、页数统计、删除指定页等 | /commons
QRCode  | 二维码 | /commons
Others  | 还有一些常用工具，就不列举了 ... | /commons


#### web 工具
Components | Description | Source
---|---|---
DTOUtils | PO to DTO 工具。使用 ***hibernate*** 的同学，估计对这个比较挠头，每次转换都费时费力，还容易出错。DTOUtils 可以实现自动转换，截断递归关联，对于级联层次很深的对象，可以指定转换深度。比目前大多数人采用 bean copy 的方案好。这个有时间我写一篇博客，详细说一下。 | /web
Spring JPA   | spring jpa 动态查询工具，可以动态组装查询条件，自动分页，很好用 | /web
Jqgird   | [Jqgrid](http://www.trirand.com/blog/?page_id=6/) 工具类，可以方便的处理查询条件。 | /web
ZTree  | [ZTree](http://www.ztree.me/v3/main.php#_zTreeInfo/) java utils ，功能强大，做后台管理用。 | /web
Fuelux Tree  | [FueluxTree](http://getfuelux.com/javascript.html#tree/) java utils ，ui 很好看，做展示用吧。 | /web
flexpaper  | [flexpaper](http://flexpaper.devaldi.com/annotate-pdf-documents-online.jsp) 在线文档展示的一种解决方案 | /web
Others  | 逐步添加 ... | /web