# 농구할래?!

농구를 사랑하는 사람들을 위한 커뮤니티 프로젝트입니다. 농구인들은 종종 리그나 특정 커뮤니티에 속하지 않으면 함께 농구를 할 친구나 다른 팀과 경기를 하는 데 어려움을 겪습니다. 이 웹 프로젝트는 이러한 어려움을 해결하기 위해 기획되었습니다. 농구인들이 함께 경기를 할 사람들을 찾고, 팀을 만들거나 소규모 농구 경기를 주선하는 등의 기능을 제공합니다. 이 프로젝트는 모바일과 웹 모두에서 사용할 수 있도록 설계되었습니다.

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
Spring 선택
file->new->spring legacy project->spring mvc project

Edit POM file
java-version, org.springframework-version, HikariCP, Mybatis, lombok, spring-test, junit, maven-compiler-plugin

Root-Context.xml edit
prereuired NameSpace {apo, beans, c, context, mybatis-spring, p} 선택택
hikariConfig, dataSource, sqlSessionFactory, mybatis-spring:scan, context:component-scan

### 2. Schedule Management

<img width="686" alt="Screenshot 2023-01-08 at 1 30 26 PM" src="https://user-images.githubusercontent.com/56284745/211180506-0b5b10f0-7bcc-4547-abf8-654624c73fb2.png">

### 3. Features

Login
- Spring Security를 사용하여 로그인 개발이 훨씬 쉬워지고 보안도 강화되었으며, 사용자 정보를 Oracle 데이터베이스에 성공적으로 업로드할 수 있었습니다.

<img width="649" alt="Screenshot 2023-01-08 at 1 37 51 PM" src="https://user-images.githubusercontent.com/56284745/211180631-6b10fcc9-8ed0-4e4a-b1fb-09030b40abd6.png">

코트 위치 등록
- Kakao 지도 API를 사용하여 사용자가 농구장 위치를 업로드해 지도 정보를 업데이트할 수 있도록 구현했습니다.

<img width="185" alt="Screenshot 2023-01-08 at 1 40 44 PM" src="https://user-images.githubusercontent.com/56284745/211180790-b579537b-477c-4f2a-a789-d93a9a695c19.png">

Create teams, Broadcast team/team members search

<img width="682" alt="Screenshot 2023-01-08 at 1 47 08 PM" src="https://user-images.githubusercontent.com/56284745/211180842-04bbce3d-ef9d-4496-b43f-c6d89989c4fe.png">

Reflective Reply system(Reply of Reply)
- Reflective Reply 시스템(답글의 답글)을 구현하면서 API, RDBMS, JPA, JQuery에 대한 이해를 더욱 깊이 있게 할 수 있었습니다.

### Spring MVC

- 웹 개발에서 MVC 패턴은 가장 많이 사용되는 패턴 중 하나입니다. 이 프레임워크는 DispatcherServlet을 중심으로 매퍼, 뷰어 등을 포함하여 동작하며, 주로 @Controller와 @RequestMapping 어노테이션에 기반을 둡니다. 특히 Spring 3.0이 도입된 이후, @Controller 어노테이션은 RESTful 웹사이트와 애플리케이션을 쉽게 만들 수 있도록 지원합니다. 이 기능은 데이터베이스와 매퍼 등과의 관계를 설정할 때 매우 유용합니다.


![Spring MVC workflow diagram](https://user-images.githubusercontent.com/56284745/211181322-4eda546e-54ef-4620-abbd-6e8cc89eb914.png)

-ref: https://www.codejava.net/frameworks/spring/how-to-enable-spring-mvc-in-webxml

### What i learned
이 프로젝트는 제 첫 번째 프로젝트였습니다. 처음에는 이 프레임워크가 얼마나 삶을 편하게 만들어주는지 잘 느끼지 못했는데, 아마도 다른 도구와 비교할 경험이 없었기 때문인 것 같습니다. 그래서 이 프레임워크가 실제로 어떻게 작동하는지, 라이브러리와 플러그인이 프로젝트에서 어떤 역할을 하는지 깊이 파고들지 않았던 것 같아요. 하지만 프로젝트를 마치고, 웹 프로젝트를 처음부터 끝까지 직접 만들어보니 Spring이라는 도구가 얼마나 매력적인지 새삼 깨닫게 되었습니다. 그래서 더 나은 개발 환경과 프로그래밍 흐름을 제공하는 프레임워크와 도구를 만드는 사람이 되면 좋겠다는 생각이 들었습니다.
