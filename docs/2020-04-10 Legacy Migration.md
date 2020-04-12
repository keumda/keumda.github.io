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
- B/E: Spring boot
- Web Server: tomcat inside springboot
- Server: cloud
- F/E: Vuejs
- Build Tool: gradle
- Datasource: mysql
- ORM: spring JPA, queryDSL
- Deployment: jenkins