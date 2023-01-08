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

![Uploading Screenshot 2023-01-08 at 1.40.44 PM.png…]()


## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 


