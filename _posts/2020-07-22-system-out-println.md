---
title: 자바 표준 출력
categories:
- Java Beginner Course
tags:
- java
- static void main
- System.out.println
---

프로그램을 접하는 가장 빠른 길은 화면에 뭔가를 그려보는 (출력하는) 것입니다.   
자바에서 출력을 담당하는 가장 심플하고 널리 쓰이는 메소드(함수)는 System.out.println 입니다.

### 출력 메소드

```java
public class JavaRunner {	
	public static void main(String[] args) {
		System.out.println("이곳에 적은 글자는 모양 그대로 화면에 출력됩니다");		
	}
}
```

### print, println, printf

비슷비슷해 보이지만, 약간씩 차이가 있습니다.

System.out.print : 출력   
System.out.println : 출력 후 줄바꿈 (엔터키 효과, 개행문자라고도 함)   
System.out.printf : 폼 출력

메소드(함수) 이름에서도 알 수 있듯이, print 는 단순히 출력만 담당하고, println은 하나의 line으로 출력하는 역할을 합니다. 그리고 printf는 form을 만들어서 출력할 수 있습니다.

printf는 C언어에서도 이와 동일한 출력함수가 있습니다.  printf 함수를 사용하여, 아래와 같은 여러 가지 폼으로 출력할 수 있습니다.


| 서식문자 | 데이터 형태 | 사용 예 |
|:---:|:---:|:---|
| %d | 정수 | printf("%d", 100); |
| %f | 실수 |  printf("%f", 0.53); |
| %c | 문자 |  printf("%c", 'A'); |
| %s | 문자열 |  printf("%s", "hello"); |

그리고, 여러 서식과 문자열을 중복하여 나열하여 아래와 같은 표현도 가능합니다.

```
printf("%d / %d = %.2f 입니다.", 36, 7, (float)36/7);
>> 36 / 5 = 5.14 입니다.
```

### 실무에서는...

여러 가지 출력 메소드가 있지만, 실무에서는 거의 println 위주로 사용합니다. 가끔, 아주 가끔 print 혹은 거의 드물게 printf를 사용하는 경우가 있지만, 사실 System.out.println 으로 화면을 출력하는 일이 거의 없기 때문에 상업적인 웹 프로그램에서는 사용하는 경우가 드뭅니다.   

자바 강의에서는 아직 웹이든 앱이든 화면이 없기 때문에 println으로 출력 결과를 확인하는 용도로 많이 사용합니다.

### 강의동영상(유튜브)

아래 그림을 클릭하면, 유튜브로 이동합니다.

[![출력해 봅시ㅏ](https://i9.ytimg.com/vi/Yijfbn5SzwA/mq1.jpg?sqp=CKi27PsF&rs=AOn4CLBJTG8zoBaRNkhrF4L--vpO0MNr3g)](https://youtu.be/Yijfbn5SzwA)
