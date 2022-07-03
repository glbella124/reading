[TOC]



# Java学习

### 一、初识Java

计算机语言经历了三代 - 机器语言，汇编语言，高级语言

Sun公司

James Gosling

![image-20220627104946269](E:\Bella\Study\reading\image\image-20220627104946269.png)

**java8 和 java9目录对比**

![image-20220627105059981](E:\Bella\Study\reading\image\image-20220627105059981.png)



#### Java体系结构

![image-20220627105152958](E:\Bella\Study\reading\image\image-20220627105152958.png)

JavaSE - 桌面应用

JavaEE - 服务器端 (网站)

#### Java特性和优势

高性能，分布式，多线程，健壮性

![image-20220627105756253](E:\Bella\Study\reading\image\image-20220627105756253.png)

#### 核心机制

##### 1.垃圾收集机制

清除不再使用的垃圾

消除了程序员回收无用内存空间的职责，

对象建立时开始监控对象的动态情况 - 对内存释放

提供一种系统级线程跟踪存储空间的分配情况

在JVM空闲时，检查并释放可被释放的存储器空间

`垃圾收集在Java程序运行中自动进行，程序员无法精确控制和干预`

GC（垃圾收集器）的自动回收，提高了内存空间的利用效率，很大程度上减少了因为没有释放空间而导致的内存泄漏

![image-20220627105959363](E:\Bella\Study\reading\image\image-20220627105959363.png)

##### 2.面试问题 - 垃圾收集器

垃圾收集器有几种

垃圾收集器底层原理剖析

垃圾收集器算法，优化

##### 3.跨平台原理

Java是解释型语言

![image-20220627104848881](E:\Bella\Study\reading\image\image-20220627104848881.png)

![image-20220627110249191](E:\Bella\Study\reading\image\image-20220627110249191.png)

Java虚拟机 - 相当于翻译官，将字节码文件翻译成当前平台认识的可执行文件

java.exe --> 底层动态调用虚拟机，JVM将字节码一行一行的解释成为当前操作系统认识的可执行文件的格式

##### 4.对比C语言跨平台原理

C语言有不同的编译器，编译后的可执行文件只能在唯一平台上运行

C语言跨平台 - 不同平台有不同的解释器，指源文件跨平台

C语言效率高

<u>通过不同平台编译器产生的可执行文件可以直接在该平台编译</u>

![image-20220627113629377](E:\Bella\Study\reading\image\image-20220627113629377.png)



#### DOS操作系统

window出现之前，当windows崩溃时，依然要用dos方式解决，是一种纯命令方式，cmd其实是windows进入dos的方式

###### 具体dos命令

```Java
//切换盘
>D:
//显示详细信息
>dir
//切换目录
>cd Bella
//退回上级目录
>cd ..
//清屏 - 未删历史记录
>cls
//创建目录
>md test
//清除文件
>rd test
//删除文件 - del后接目录，只删除内部文件
>del demo.txt

```

### Java项目部署到Linux服务器

https://zhuanlan.zhihu.com/p/419109069

### JDK和JRE

JDK : Java Development kit ---> 编写Java程序的程序员使用的软件

JRE: Java Runtime Environment --> 运行Java程序的用户使用的软件
