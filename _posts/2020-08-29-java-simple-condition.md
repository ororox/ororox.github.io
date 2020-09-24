---
title: 자바 조건문 1, if 조건문
categories:
- Java Beginner Course
tags:
- java
- static void main
- if
---

if를 이용한 조건문은 단지 자바에서만 쓰이는 것이 아니라, 거의 모든 프로그래밍 언어에서 사용하는 가장 중요한 조건문입니다.   

### 문제

다음 코드를 보고 출력을 예상하시오.

```java
public class JavaRunner01 {

	public static void main(String[] args) {
		
		/* 입력부 */
		int firstNumber = 2;

		/* 연산부 */
		if (firstNumber > 0) {
			System.out.println("첫번째 숫자는 3보다 크다");		// 출력부
		}
		
		if (firstNumber <= 1) {
			System.out.println("첫번째 숫자는 1보다 작거나 같다");	// 출력부
		}
		
		if (firstNumber == 2) {
			System.out.println("첫번째 숫자는 2이다");		// 출력부
		}
	}
}
```
### 소스코드 설명

if 뒤에 나오는 괄호의 패턴은 자바에서 흔히 사용하는 관습(코드 컨벤션)입니다. 왜 그렇게 사용하는가? 그런 건 없습니다. 그냥 자바 프로그래머들의 관습이자 습관입니다.   

만일, 같은 코드라도 C언어 사용자는 아래와 같이 괄호를 남기는 관습을 가지고 있습니다.

```c
if (firstNumber > 0)
{
     printf("첫번째 숫자는 3보다 크다");
}
```

그리고 파이썬은 괄호가 없이 띄어쓰기로 괄호를 대체합니다. 그리고 문장을 끝내는 세미콜론(;)도 없습니다.

```python
if firstNumber > 0:
    print("첫번째 숫자는 3보다 크다")
```

**if 문은 조건을 만족하면, 내부에 연산이 실행**되고, 그렇지 않으면 아무것도 하지 않고 그냥 지나쳐갑니다.

### 문제 정답

아래를 마우스로 긁어보시면 정답이 있습니다.

---

<span style="color: white">
첫번째 숫자는 3보다 크다   
첫번째 숫자는 2이다   
</span>

---

### 다른 코드

출력부를 분리한 스타일로 만든 코드는 아래 gist 링크에 있습니다.  
[자바 연습문제 2](https://gist.github.com/ororox/e0e7695218db23e5bbc179b82718dabf)
