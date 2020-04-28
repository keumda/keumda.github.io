---
layout: default
title: Spring Framework 레가시 시스템 마이그레이션 
date: 2020-04-10 02:22
nav-order: 4
description: ""
---

# 아키텍처 정의
AS-IS
- B/E: Spring framework 4.3, java 1.7
- Web Server: Tomcat 7
- Server: (?)
- F/E: jsp, jquery
- Build Tool: maven (?)
- Datasource: mysql
- SQL Mapper: mybatis
- Deployment: jenkins

TO-BE
- B/E: Spring boot 2.0 (which supports Spring 5)
- Web Server: tomcat inside springboot
- Server: cloud
- F/E: Vuejs
- Build Tool: gradle
- Datasource: mysql
- ORM: spring JPA, queryDSL
- Deployment: jenkins

# 마이그레이션 참고 링크
- https://d2.naver.com/helloworld/5626759 (Maven to Gradle, SpringMVC to SpringBoot)
- https://jojoldu.tistory.com/10
- https://kamang-it.tistory.com/entry/IntelliJmaven%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-intelliJ%EC%97%90-%EC%9E%84%ED%8F%B4%ED%8A%B8%ED%95%98%EA%B8%B0 (Eclipse to IntelliJ)
- MyBatis to JPA
- Hosting to AWS(or GCP)
- https://aws.amazon.com/ko/getting-started/tutorials/get-a-domain/ (Domain 설정)
