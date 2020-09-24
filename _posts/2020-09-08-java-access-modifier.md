---
title: 자바 접근제어자, Access Modifier
categories:
- Java Beginner Course
tags:
- java
- private
- public
- access modifier
---

자바 코드 내부에 있는 **변수와 메소드**는 **기능이나 업무영역**에 따라  **클래스와 패키징**으로 적절하게 분류되어 묶여 있습니다.   

따라서, 자바 코드 내에 있는 변수와 메소드에  접근하여 값을 조회하거나 변경하는 것에 대하여 적절한 제어가 필요합니다. 이러한 접근 제어가 제대로 되어 있지 않을 경우에는 여러 곳에서 마구잡이로 변경이 일어나기 때문에 프로그램의 에러를 찾아내는 일이 더욱 어려워집니다.

자바에서는 이러한 접근 제어를 위해 private, default, protected, public 네 가지 방식을 사용하며, 차례로 접근범위가 넓어집니다.   

> private < default <  protected < public

### private

접근제어자가 private으로 설정되면, private이 붙은 변수, 메소드는 해당 클래스 내에서만 접근 가능합니다.   

```java
public class Book {
	
	private int page;

	private String getTitle() {
		System.out.println("This is a book");
	}

}
```   

page라는 변수와 getPage()라는 메소드는 클래스 내부에서만 사용 가능하고(접근 가능하고), 클래스 외부에서는 변수의 값을 조회하거나 메소도를 호출하는 것이 막혀 있습니다.


### default

접근제어자가 있어야 할 자리에 아무것도 적지 않는다면, 그것은 default로 간주합니다. default는 **같은 패키지** 안에 있는 클래스에서 접근 가능합니다. (**하위 패키지 접근 불가**)   

```java
package com.library

public class Book {
	
	int page = 364;
	...
	
}
```

```java
package com.library

public class ApplicationRunner {
	public static void main(String[] args) {
		
		Book novel = new Boo();
		System.out.println(novel.page)

	}
}
```

### protected

protected가 붙은 변수나 메소드는 **같은 패키지** 안(**하위 패키지 불가**)에 있는 클래스 혹은 **상속받은 클래스**(외부도 상관없음)에서 접근 가능합니다. 아직 상속이라는 개념을 배우지 않은 상태이므로, 이후에 예제가 나오면 다시 배우도록 합시다. 사실, 특별한 경우가 아니면, 자주 사용하지 않는 편이라서, 굳이 한 번에 다 욕심 낼 필요는 없습니다.     


### public

변수나 메소드의 경우 public이 붙으면, 어디서든 접근하여 사용가능합니다. 그 만큼 관리가 힘들어지겠지요.   

### 실제 코드

실무에서는 관리 편의를 위해 변수는 private, 메소드는 public으로 두는 경우가 거의 대부분입니다.   
default는 코드를 대충 만든 경우에 자주 발생하며, 왠만하면 private/public 두 가지로 구분해서 꼼꼼하게 코딩하는것이 정석입니다.   
필요에 따라 가끔 protected를 쓰거나, 매우 드물게 일부러 default 상태로 두는 경우를 제외하고는 거의 대부분 아래와 같은 코드 스타일로 클래스를 구성합니다.

```java
package com.library.book;

public class Book {
	
	private int page;
	private String title;
	private String authNm;
	
	public int getPage() {
		return page;
	}
	public void setPage(int page) {
		this.page = page;
	}
	public String getTitle() {
		return title;
	}
	public void setTitle(String title) {
		this.title = title;
	}
	public String getAuthNm() {
		return authNm;
	}
	public void setAuthNm(String authNm) {
		this.authNm = authNm;
	}	
}
```
