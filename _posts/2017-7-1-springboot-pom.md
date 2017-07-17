---
layout: post
title:  "Springboot-pom"
categories: springboot
tags:  springboot pom
author: mengyang
---

* content
{:toc}
springboot_pom.xml



# springboot快速搭建地址

[走你](http://start.spring.io/)

# pom.xml
```xml
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/maven-v4_0_0.xsd">
  <modelVersion>4.0.0</modelVersion>
  <groupId>com.xmy</groupId>
  <artifactId>springboot</artifactId>
  <packaging>war</packaging>
  <version>0.0.1-SNAPSHOT</version>
  <name>springboot Maven Webapp</name>
  <url>http://maven.apache.org</url>
  <parent>  
        <groupId>org.springframework.boot</groupId>  
        <artifactId>spring-boot-starter-parent</artifactId>  
        <version>1.4.0.BUILD-SNAPSHOT</version>  
    </parent>  
  <dependencies>
    <dependency>  
            <groupId>org.springframework.boot</groupId>  
            <artifactId>spring-boot-starter-web</artifactId>  
        </dependency>  
  </dependencies>
  <build>
    <finalName>springboot</finalName>
    <plugins>  
            <plugin>  
                <groupId>org.springframework.boot</groupId>  
                <artifactId>spring-boot-maven-plugin</artifactId>  
            </plugin>  
        </plugins>  
  </build>
  <!-- Add Spring repositories -->  
    <!-- (you don't need this if you are using a .RELEASE version) -->  
    <repositories>  
        <repository>  
            <id>spring-snapshots</id>  
            <url>http://repo.spring.io/snapshot</url>  
            <snapshots><enabled>true</enabled></snapshots>  
        </repository>  
        <repository>  
            <id>spring-milestones</id>  
            <url>http://repo.spring.io/milestone</url>  
        </repository>  
    </repositories>  
    <pluginRepositories>  
        <pluginRepository>  
            <id>spring-snapshots</id>  
            <url>http://repo.spring.io/snapshot</url>  
        </pluginRepository>  
        <pluginRepository>  
            <id>spring-milestones</id>  
            <url>http://repo.spring.io/milestone</url>  
        </pluginRepository>  
    </pluginRepositories>  
</project>

```