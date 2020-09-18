---
title: 자바 조건문 2, if...else 조건문
categories:
- Java Training
tags:
- 자바연습
---

두 가지 조건에 따른 분기가 필요한 경우에는 if... else 조건문   
여러가지 조건에 다른 분기가 필요한 경우에는 if... else if.. else 조건문을 사용합니다.   

### 문제

다음 코드를 보고 출력을 예상하시오.

```java
public class JavaRunner02 {

	public static void main(String[] args) {
		
		/* 입력부 */
		int firstNumber = 2;
		int secondNumber = 3;
	

		/* 출력변수 */
		String prtStr1;
		String prtStr2;


		/* 연산부 */
		if (firstNumber >= 2 ) {
			prtStr1 = "첫번째 숫자는 2보다 크거나 같다";
		} else {
			prtStr1 = "첫번째 숫자는 2보다 작다";
		}
		
		if (secondNumber > 0 ) {
			prtStr2 = "두번째 숫자는 0보다 크다";
		} else if (secondNumber >= 1) {
			prtStr2 = "두번째 숫자는 1보다 크거나 같다";
		} else {
			prtStr2 = "두번째 숫자는 음수이다";
		}


		/* 출력부 */
		System.out.println("***************");
		System.out.println(prtStr1);
		System.out.println(prtStr2);
		System.out.println("***************");
	}
}
```
### 소스코드 설명

이번에는 출력부에서 출력을 담당하기 위하여 코드를 조금 더 다듬은 형태입니다.   
조건이 붙는 코드에서는 문자열(String) 변수에 값만 대입하고, 대입한 값은 프로그램 마지막에 출력하도록 하였습니다.   

실제로 입력부는 사용자의 입력을 받는 부분으로 바꿀 수 있고, 출력부는 나중에 화면에서 출력하는 형태와 유사하게 구성했습니다.
<br/>
조건이 많아질 경우, 아래와 같이 가운데 있는 **else if**의 갯수를 늘리면 됩니다.
```java
if ( 조건 1 ) {
	...
} else if ( 조건 2 ) {
	...
} else if ( 조건 3 ) {
	...
} else if ( 조건 4 ) {
	...
} else if ( 조건 5 ) {
	...
} else {
	...
}
```   
마지막에 나오는 **else**는 모든 조건에 해당하지 않은 경우에 실행하도록하는 **필수 마침구문**입니다.

참고로 위에 나온 "두 번째 숫자에 대한 조건문은 **잘못 만든 로직**"입니다. 이번 문제의 핵심은 출력을 예상하는 것이며, 출력이 나오는 것과 프로그램의 로직이 맞고 틀림은 다른 문제입니다.   
**유능한 프로그래머**는 단순히 프로그램을 만드는 것 뿐만 아니라, **로직(알고리즘)이 맞다 틀리다를 판단할 수 있어야** 합니다.

올바른 프로그램은 아래 gist 링크에 있습니다.   
[자바 연습문제 3](https://gist.github.com/ororox/0a7a74c1ede8b793032a7f1c080c6c61)


### 문제 정답

아래를 마우스로 긁어보시면 정답이 있습니다.

---

<span style="color: white">
`***************`   
첫번째 숫자는 2보다 크거나 같다   
두번째 숫자는 0보다 크다   
`***************`
</span>

---
