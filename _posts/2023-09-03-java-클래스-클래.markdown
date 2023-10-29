---
layout: post
title:  "클래스"
date:   2023-09-03
last_modified_at: 2018-09-20
categories: [Jekyll Paper]
tags: [Getting Start]
---
### 1.Class/클래스
---
##### Car.java라는 javaclass생성
```
String type; // 엔진 종류
int price; // 가격
String brand; // 브랜드 명
```
###### // 객체 생성
###### // Car클래스의 a7이라는 객체 생성
```
Car a7 = new Car();
 
a7.type = "deissel";
a7.brand = "audi";
a7.price = 100000000;
```
###### a7이라는 객체 프린트
```
System.out.println("a7의 엔진 타입 " + a7.type);
System.out.println("a7의 브랜드 " + a7.brand);
System.out.println("a7의 가격 " + a7.price);
```
