---
layout: post
title: linux部署到tomcat可能使用到的命令
category: linux
tags: [linux, java, tomcat]
---


最近在服务器的tomcat上部署项目的时候，使用到了几个查询命令，记录如下：

1.netstat -anp | grep :8080 查看使用端口号8080的进程，grep起到筛选作用

2.telnet 127.0.0.1 8080 查看本机的tomcat是否启动

3.ps aux | grep 4151 查看某个进程的信息

4.less logs/catalina.out 查看tomcat的控制台日志，使用q退出，其中logs为/tomcat/logs目录，使用q退出

5.tail -f logs/catalina.out 查看tomcat控制台日志， ctrl+c退出

6.history 查看前面使用过的命令


