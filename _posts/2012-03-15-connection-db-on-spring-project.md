---
layout: post
title: Spring mvc项目连接数据库
category: spring
tags: [Spring, DB]
---


使用spring连接mysql数据库。
1.添加mysql的jar包以及c3p0的jar包(该jar包主要用于数据源，如果使用别的数据源可以修改)。在pom.xml中添加如下依赖：
	
	<!-- 用于spring访问数据库 -->
	<dependency>
		<groupId>org.springframework</groupId>
		<artifactId>spring-jdbc</artifactId>
		<version>${spring.version}</version>
	</dependency>

	<dependency>
		<groupId>c3p0</groupId>
		<artifactId>c3p0</artifactId>
		<version>0.9.1.2</version>
	</dependency>

	<dependency>
		<groupId>mysql</groupId>
		<artifactId>mysql-connector-java</artifactId>
		<version>5.1.6</version>
	</dependency>


2.在applicationContext.xml中配置数据源dataSource。

3.创建数据库表 tb_user.sql

4.新建对应bean


