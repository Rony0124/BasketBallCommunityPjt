# 농구할래?!

Basketball community project for basketball lovers. Ballers were finding it hard to have basketball mates and have games with another team 
unless they are in a league or certain community. This web project is to resolve their hardships through helping them find people to play with, 
create a team, small basketball game, etc. 

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

## development


### 1. How to set Spring

Move to eclipse installation folder -> fix eclipse.ini

-vm
C:\Program Files\Java\jdk1.8.0_221\bin

UTF-8 setting
workspace, web(html, css, jsp)

install Spring plug-in in eclipse
https://download.springsource.com/release/TOOLS/update/e4.12/
Help->install new Software

Check Tomcat setting
windows->preference->server->runtime environment->add

Create project
Select Spring perspective
file->new->spring legacy project->spring mvc project

Edit POM file
java-version, org.springframework-version, HikariCP, Mybatis, lombok, spring-test, junit, maven-compiler-plugin

Root-Context.xml edit
Choose prereuired NameSpace {apo, beans, c, context, mybatis-spring, p}
hikariConfig, dataSource, sqlSessionFactory, mybatis-spring:scan, context:component-scan

### 2. Schedule Management

<img width="686" alt="Screenshot 2023-01-08 at 1 30 26 PM" src="https://user-images.githubusercontent.com/56284745/211180506-0b5b10f0-7bcc-4547-abf8-654624c73fb2.png">

### 3. Features

Login
- Using Spring Security, log in development became much easier and more secure, and was able to successfully upload user info into oracle database.

<img width="649" alt="Screenshot 2023-01-08 at 1 37 51 PM" src="https://user-images.githubusercontent.com/56284745/211180631-6b10fcc9-8ed0-4e4a-b1fb-09030b40abd6.png">

Court Location registration
- By using Kakao map api, enabled for user to update map info uploading basketballl location.

<img width="185" alt="Screenshot 2023-01-08 at 1 40 44 PM" src="https://user-images.githubusercontent.com/56284745/211180790-b579537b-477c-4f2a-a789-d93a9a695c19.png">

Create teams, Broadcast team/team members search

<img width="682" alt="Screenshot 2023-01-08 at 1 47 08 PM" src="https://user-images.githubusercontent.com/56284745/211180842-04bbce3d-ef9d-4496-b43f-c6d89989c4fe.png">

Reflective Reply system(Reply of Reply)
- this help me deep-dive into understanding of api, RDBMS, JPA, JQuery

### Spring MVC

- In web-development, i couldn't help but notice MVC Pattern is one of the most commonly used pattern on Web project. 
this framework works around DispatcherServlet with mapperss, viewers and so on. mostly based on the @Controller and @RequestMapping annotations. and As of introduction of Spring 3.0, the @Controller annotation allows develops to create RESTful Web sites and applications. This feature comes in handy when creating relationships between Database and Mappers and others.


![Spring MVC workflow diagram](https://user-images.githubusercontent.com/56284745/211181322-4eda546e-54ef-4620-abbd-6e8cc89eb914.png)

-ref: https://www.codejava.net/frameworks/spring/how-to-enable-spring-mvc-in-webxml
