---
title: 자바 반복문 3, 기타
categories:
- Java Beginner Course
tags:
- java
- loop
- do while
---

자바에는 문법은 존재하지만 활용빈도가 적은 반복구문들이 있습니다.

### for each

J2SE 5.0 부터 등장한 새로운 구문입니다.

```java
String[] numbers = {"one", "two", "three"};
for(String number: numbers) {
    System.out.println(number);
}
```

뭐 이렇게 생긴 코드이긴 한데, 조회할 때 for 구문을 짧게 줄여주는 코드라서 많이 쓰일 줄 알았는데,  
생각만큼 많이 쓰진 않는 듯 합니다.  
조회하기에는 좋지만, 데이터를 가공하기에 번거롭기 때문에 과거의 관습적인 코딩을 쓰는경우가 여전히 많습니다.


### do... while

while문을 사용하기 전에 반드시 실행되어야 할 것이 있다면, 미리 실행하고, while 문 안에서 Loop를 돌기 위해서 사용하기 위해서 만들었지만, while 문 사용빈도가 적다보니... 심지어 do... while 구문이 있는지도 모르는 사람도 많습니다.   

```java
do {
  System.out.println("초기화 중입니다...");
} while (num <= 5);
  System.out.println("program and.... ");
}
```

### break, continue

while 구문을 설명할 때 같이 설명했어야 하지만...

아... 번거롭습니다. while 문을 맛깔스럽게 사용하기 위해서는 적절한 break 그리고 때에 따라서는 continue라는 구문을 적절히 사용할 수 있어야 합니다.

저도 이 부분은 설명이 번거롭기에...   
[점프 투 자바: while 문](https://wikidocs.net/212){:target="_blank} 내용을 참조하시기 바랍니다.
