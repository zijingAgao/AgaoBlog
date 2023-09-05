---
title: JAVA 安装使用
---
Oracle Java
### 一、JAVA 下载
    官网地址：https://www.oracle.com/cn/java/technologies/downloads/

根据所需系统版本下载对应版本

    eg: windows-64bit: 下载 jdk-8u381-windows-x64.exe


### 二、JAVA 安装
> 建议有专门存放开发环境的路径：

    eg:

    D:\Environment\java\jdk

    D:\Environment\java\jre


1.双击打开.exe文件，选择上述安装路径。

2.安装JDK时，会打开安装JRE的引导，选择上述安装路径。

### 三、配置环境变量

> eg: windows 10 (T_T)

右键此电脑->属性->高级系统设置->环境变量->系统变量（注意不是用户变量）

    添加如下配置（Key: Value）：Path是已有key，添加value即可
    
    JAVA_HOME : D:\Environment\java\jdk
    CLASSPATH : .;%Java_Home%\bin;%Java_Home%\lib\dt.jar;%Java_Home%\lib\tools.jar
    Path : %Java_Home%\bin
    Path : %Java_Home%\jre\bin

### 四、检查
Win+R ，输入cmd ，回车
```shell
# 看到java版本号即jdk配置成功
java -version  

#看到可执行的选项即jre配置成功
javac
```

### 五、备注
可能的问题：
反复确认环境变量配置的路径：多了个\ 少了个\ 少了个. 等