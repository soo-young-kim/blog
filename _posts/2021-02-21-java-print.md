---
layout: post
title: Java 주석
date: 2021-2-21
image_preview: https://t1.daumcdn.net/cfile/tistory/2319C74A562F295521
---
##1

```java
System.out.print : 
int num = 10;
System.out.print("num은 " + num);
System.out.print("입니다"); //로 입력할경우 줄이 안바뀐다

----> num은 10 입니다
```
##2
 print를 println으로 바꾸면
 ```java
 int num = 10;
System.out.println("num은 " + num);
System.out.println("입니다"); //로 입력하면 줄이 바뀜

---> num은 10
      입니다
```
3
------

- print에서 줄바꿈을 하는 방법
```java
int num = 10;
System.out.print("num은 " + num);
System.out.print("\n입니다");

---> num은 10
     입니다
```
```
\n : 줄바꿈
\t : 탭(tab)
\" : 큰 따옴표
\\ : 역슬래쉬
```
t는 탭처럼 들여쓰기나 띄어쓰기가 되고



\"는 큰따옴표 " 를 온전히 문자열 안에서 사용하고 싶을 떄 사용



컴파일할 때 큰 따옴표를 문자열을 표현하는 도구로 인식하기 때문에
역슬래쉬를 써야한다

---
그가 물었다. "너는 누구니?"



라는 문장을 표현하고 싶으면


```java
System.out.println("그가 물었다. \"너는 누구니?\"");
```

4 
---------
- printf 
```java
System.out.printf("더하기 %d + %d = %d", 10, 20, (10+20));

--> 더하기 10+20 = 30
```
%d = <span style = "color : orange">서식문자 또는 변환문자 (정수와 10진수)</span>
%f : 실수
%c : 문자
%s : 문자열 (2글자 이상의 문자)
%d : 10진수 정수
%o : 8진수 정수
%x : 16진수 정수
```java
int num = 10;
System.out.printf("내 이름 : %s \n", "프로"); //문자열은 큰 따옴표로
System.out.printf("알파벳 : %c \n", 'P'); //문자는 작은 따옴표로
System.out.printf("실수는 %f \n", 10.10);
System.out.printf("정수표기 : %d \t %o \t %x \n", num, num, num);
```


