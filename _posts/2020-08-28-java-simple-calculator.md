---
title: 간단한 자바 계산기
categories:
- Java Training
tags:
- 자바연습
---

제목은 간단한 자바 계산기이지만, 처음 자바를 접하는 분들에게는 매우 어려울 수 있는 예제입니다.

### 문제

소스 코드에서 1~5 번에 코멘트를 제거하고 코딩을 완성하여, 아래 콘솔과 같은 출력이 나오게 하시오.

```java
public class JavaRunner {

	public static void main(String[] args) {
		
		/* 입력부 */
		// 현재는 내부에 있으나, 향후 사용자 입력을 받을 예정
		int firstNumber = 2;
		int secondNumber = 3;

		/* 연산부 */
		// 내부 연산으로 사용
		int sumOfNumbers = firstNumber + secondNumber;
		int subtractOfNumbers = firstNumber - secondNumber;
// 1.		int powerOfNumbers = 
// 2.		double dividOfNumbers = 
		
		/* 출력부 */
		// 현재는 콘솔 출력이지만, 향후 화면으로 구현
		System.out.println("***************");
// 3. 여기에 출력 제목 작성
		System.out.println("***************");
		System.out.println("");
		System.out.println("두 숫자의 합은: " + sumOfNumbers + "입니다.");
		System.out.println("두 숫자의 차는: " + subtractOfNumbers + "입니다.");
// 4. 여기에 출력 모양 작성 (곱셈)
// 5. 여기에 출력 모양 작성 (나눗셈: 나눗셈은 매우 어려움)
	}
}
```

![java-runner01]({{ 'assets/images/post/java-runner01.png' | relative_url }})

### 소스코드 설명

자바에서는 두 가지 형태로 코멘트(주석)를 남길 수 있습니다.
여러 줄에 걸쳐서 코멘트를 남기는 경우에는 아래와 같이 하며,

```java
/* 프로그램 사용법
  작성자 : ororox
  작성일 : yyyy-mm-dd */
```

한 줄로 코멘트를 남길 경우에는

```java
// 여기에 적습니다.
// 간단하게 적을 때 주로 사용합니다.
```

**입력부**에서는 현재는 소스코드 내부에서 숫자를 입력하지만, 나중에는 외부에서 숫자를 받아올 수 있습니다.   
**연산부**는 내부에 숨겨진 코드이며, 실제로 계산 또는 로직을 수행하는 역할을 합니다.   
**출력부**에서는 결과를 출력합니다. 대부분 웹 화면에서 표현되지만, 아직 우리는 화면을 그리는 단계는 아니므로, 콘솔창에 결과를 프린트 합니다.

### 문제 정답

정답은 [여기](https://gist.github.com/ororox/d9acf4a4254a5dd65f0aca1b12fa9acb){:target="_blank"}에 있습니다.   
처음하는 프로그래밍이므로 너무 고민하기 보다는 해답을 보고, 이해하는 것도 좋습니다.   
실무에서 처음부터 무리한 코딩을 요구하는 경우는 없습니다. 대부분 다른 사람이 만든 코드를 이해하는 것에서 출발합니다. 그래서, 프로그래밍은 약간의 도재식 수업이 필요합니다.
