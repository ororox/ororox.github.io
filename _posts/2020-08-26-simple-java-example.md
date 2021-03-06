---
title: 간단한 덧셈 예제
categories:
- Java Beginner Course
tags:
- java
- static void main
---

앞에서 봤던 [자바 실행 클래스](https://ororox.github.io/java%20beginner%20course/JavaRunner/){:target="_blank"} 안에서 간단한 프로그램을 만들어 봅시다.


### 소스코드

```java
public class JavaRunner {	
	public static void main(String[] args) {		
		int a, b, c;
		a = 1;
		b = 2;
		c = a + b;		
		System.out.println(c);		
	}
}
```

원래 있던 코멘트 자리를 지우고, 위에 작성한 코드로 대체하고, 반드시 **저장**을 합니다. 이클립스는 저장과 동시에 프로그램 실행이 가능한 파일로 컴파일합니다.

### 실행과정

실행할 파일을 선택한 후, 마우스 "우클릭"   

> Run As > Java Application

선택하여 프로그램을 실행하면, **console**에 **3**이라는 숫자가 출력됩니다.


### 소스코드 설명

프로그램 소스코드를 하나씩 살펴봅시다. 프로그램 소스코드 외부는 나중에 다시 설명하기로 하겠습니다.
어쨌든 이부분은 항상 이렇게 사용하고, **JavaRunner**라는 부분만 이름처럼 바꿔가며 사용한다고 생각해도 됩니다. (아직까지는 말이지요)

```java
public class JavaRunner {	
	public static void main(String[] args) {		
		...	
	}
}
```

우리가 주목해서 볼 부분은 아래 코드입니다.

```java
		int a, b, c;
		a = 1;
		b = 2;
		c = a + b;		
		System.out.println(c);	
```

**int**는 **Integer**의 줄임말로서, int 뒤에 글자를 적으면, **정수**를 저장할 수 있는 저장소 이름이 됩니다. 이러한 저장소를 변수(variable)라고 합니다. 쉼표로 구분하여, 여러 개를 동시에 **선언**하여 사용하기도 하고, 하나씩 각 줄로 써도 무방합니다.

"**=**(등호)" 기호는 같다는 표시가 **아닙니다**. 왼쪽의 변수(저장소, 메모리)에 오른쪽 숫자를 대입(입력)한다는 뜻입니다.

```java
a = 1;
```

이라고 하면, "a"라는 이름표를 가진 변수에는 숫자(정수) "1"을 저장한다는 뜻입니다.

참고로, "같다"라는 뜻의 기호는 등호를 두 개 붙여서 "**==**" 를 사용하여 비교합니다.

뒤에 세미콜론(;)은 마침표 역할을 합니다. 문장에서 사용하는 마침표(.)는 프로그램에서 다른 용도로 사용하고 있어서, 세미콜론이 마침표 역할을 하는 것입니다.

a에는 1을 저장했고, b에는 2를 저장했습니다. 그러면,

```java
c = a + b;
```

라고 하면, c에는 a에 저장한 값과 b에 저장한 값을 합해서, c에 저장한다는 뜻입니다.

마지막으로,

```java
System.out.println(c);
```

를 이용하여 c에 들어있는 값을 출력합니다.
