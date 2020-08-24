---
title: 자바 실행 클래스
categories:
- Java Training
tags:
- 자바연습
---

자바코드 실행을 **반드시** 아래와 같은 코드가 필요합니다. 

```java
public class JavaRunner {

	public static void main(String[] args) {
		
		System.out.println("Hello World!");
		
	}
}
```

보통은 이런 코드가 프로그램 **실행의 시작점**이라고 볼 수 있지요.

```java
public class JavaRunner {

	public static void main(String[] args) {
		
        // 여기서부터 코드를 적으면 실행가능

	}
}
```

"// 여기서부터 코드를..."   
이 부분은, 프로그램 실행에 영향을 주지 않는 코드라인입니다. **코멘트(Comment)** 라고 하며, 주로 프로그래머가 간략한 설명 등을 남기는 용도로 사용합니다.   
코멘트는 "주석"이라고도 하는데, 일본식 한자어를 음차한 표현입니다.

**Java Runner**라는 클래스 이름은 JavaTest, JavaRun 등 편리한 이름 아무거나 적어도 상관없습니다. 단, 자바 언어에서 이미 사용하고 있는 예약어만 아니면 됩니다.
