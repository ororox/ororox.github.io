---
title: 자바 메소드, method
categories:
- Java Training
tags:
- 자바연습
---

다른 언어에서는 함수(function)이라고 부르는 것을 자바에서는 메소드(method)라고 부릅니다.    

특별히 이름을 다르게 한 이유는 없습니다. 그냥 좀 튀고 싶었나 봅니다.

### 함수, 메소드

수학에서 말하는 함수는 아래와 같은 그림으로 설명합니다.   

![함수](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3b/Function_machine2.svg/220px-Function_machine2.svg.png)   

프로그래밍에서 말하는 함수도 이것과 크게 다르지 않습니다. 대개 입력, 연산, 출력 이렇게 3개의 구성요소를 가지고 있습니다.

가장 일반적인 자바 메소드의 모습은 이렇습니다.

```java
public int sum(int a, int b) {
    return a+b;
} 
```

위의 예제를 일반적인 모습의 선언으로 바꾸면 아래와 같습니다.

```java
접근제어자 리턴자료형 메소드명(입력자료형1 입력변수1, 입력자료형2 입력변수2, ...) {
    ...    
    return 리턴값;
}
```
여기서 돌려줄 값(리턴값)이 없는 경우에는 return 문은 적지 않습니다.


### 메소드를 사용하는 이유
