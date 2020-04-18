---
layout: default
title: Spring Boot와 AWS 웹서비스 구현 Pilot
nav_order: 2
description: ""
---

# IntelliJ 설정 시작

---

## Getting started (from 2020.04.01)
jojoldo 블로그 참고

*[참고 git repo](https://github.com/jojoldu/freelec-springboot2-webservice.git)  
*[참고 blog](https://jojoldu.tistory.com/)  

### IntelliJ로 Gradle 프로젝트 생성

### Springboot Testcode 작성
* JUnit Annotation (@Test, )

### TDD로 프로젝트 시작하고 단위테스트 작성 (Junit)
* AssertThat in AssertJ
* Lombok Annotation (@NoArgsConstructor, @Getter, @Builder)

### JPA 시작하기
* JPA/Hibernate/Spring Data Jpa
* SQL Mapper vs. ORM (MyBatis vs. JPA)
* QueryDSL

* 패러다임 불일치 (관계형 DB에 어떻게 저장할지 vs. 기능과 속성을 관리하는 객체지향)
* 단순 CRUD 반복작업
* 구현체 교체의 용이성 (Hibernate, Jedis, Redis, Lettuce)
* 저장소 교체의 용이성 (MySql, MongoDB)

* JPA Annotation (@Entity, )
단, Entity class에서는 Setter를 생성하지 않는다
기본 Repository가 필수적으로 함께 위치

* DDD - DDT Start (최범균)
* Dirty Checking
- JPA의 영속성 Context
- EntityManager가 Entity를 영구 저장
- Transaction이 끝나는 시점에 일괄 반영
- 일부만 반영하고 싶을 경우 별도 설정 (@DynamicUpdate)
* Transactional

* h2 console - gradle build issue

* JPA Auditing - 생성/수정시간 자동화
* LocalDateTime Class

## Spring MVC vs. Spring Boot
* Spring Annotation (@Service, @Transactional)

## Layers
1. Web Layer
2. Service Layer
비지니스로직을 처리하지 않고, Transaction 도메인 간의 순서 보장의 역할
3. Repository Layer
4. Dtos
Entity 클레스와 비슷하지만, view를 위한 클래스로 controller에서 쓰이며 자주 변경
Entity 클레스의 일부만 사용
5. Domain
실제 비지니스 로직을 처리

