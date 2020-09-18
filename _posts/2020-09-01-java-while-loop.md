---
title: 자바 반복문 1, while
categories:
- Java Training
tags:
- 자바연습
---

while 반복문은 의외로 자바에서 많이 쓰지 않는 반복문입니다.   

초보자 입장에서는 직관적으로 이해하기 쉬운 구문이라서 많이 사용할 것 같지만, 실제 실무에서는 의외로 드물게 사용하는 편입니다.   

아래 콘솔창 출력처럼 나오게 프로그램을 만들어 보시오.   
![]({{ 'assets/images/post/10-times-print.png' | relative_url }})

### while 구문

while은 영어로 "~하는 동안"라는 뜻이 있습니다. 그래서 프로그램에서도 똑같이 조건이 참(true)인 경우에 계속해서 반복수행하는 기능으로 사용하고 있습니다.   
위에서 보는 것처럼 10번 같은 동작을 수행하려면 아래와 같이 프로그램을 만들면 됩니다.

```java
public class JavaRunner03 {

	public static void main(String[] args) {
		
		int i = 0;
		while( i < 10 ) {
			System.out.println("이 문장이 10번 출력되도록 하시오");
			i++;
		}
	}
}
```

### 소스코드 설명

**i** 라는 변수명은 정수(integer)라는 의미도 있지만, 인덱스(index)라는 의미에서 **i** 라는 변수명을 많이 사용합니다. 일종의 관습입니다.     

* i++ 는 1씩 증가시킨다는 의미입니다.   

"++i"로 사용해도 10번 반복합니다. "++i "와 "i++" 의 차이는 "++i"는 변수의 값을 사용하기 전에 미리 증가시키는 것이고, "i++"는 변수의 값을 사용한 후에 1 증가시킨다는 의미입니다.

초기값을 0으로 시작해서,10보다 작을 때까지, 즉  0 ~ 9까지 증가하는 동안 총 10번 반복하는 구문입니다.   

초기값을 1로 시작해서 1~10까지 증가하는 코드로 만들 수도 있다.

```java
public class JavaRunner03 {

	public static void main(String[] args) {
		
		int i = 1;
		while( i <= 10 ) {
			System.out.println("이 문장이 10번 출력되도록 하시오");
			i++;
		}
	}
}
```

하지만, 이것도 프로그램에서는 관습적으로 시작을 0부터 시작합니다. 그래서, 0 ~ 9까지 10번 반복하도록 하는 것이 일반적인 **코딩스타일**입니다.

### 무한 루프(Loop)

자바 프로그램에서 while문을 꺼려하는 이유는 자칫 실수하면, 무한 루프에 빠지기 때문입니다.   
위에서 설명한 코드에서, i++를 깜빡하고 빠뜨리는 순간, 이 코드는 무한루프에 빠집니다.
i++ 부분을 지우는 대신, comment 처리하면, 없는 것처럼, 마치 지운 것처럼 작동합니다.   
재미로 한 번 실행시켜 보시는 것도 좋습니다. (멈추는 방법은 하단에 있습니다)   

```java
public class JavaRunner03 {

	public static void main(String[] args) {
		
		int i = 1;
		while( i <= 10 ) {
			System.out.println("이 문장이 10번 출력되도록 하시오");
			//i++;
		}
	}
}
```

이클립스에서는 프로그램이 시작되면, 빨간색 정지버튼이 활성화됩니다. 멈추지 않고, 계속 프로그램이 도는 경우, 빨간색 정지버튼을 클릭해서 멈출 수 있습니다.

![]({{ 'assets/images/post/infinite-loop.png' | relative_url }})
