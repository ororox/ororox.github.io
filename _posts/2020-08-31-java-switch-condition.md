---
title: 자바 조건문 3, switch/case
categories:
- Java Beginner Course
tags:
- java
- switch
- case
---

자바에서는 여러가지 조건에 따른 분기를 위해서 switch/case를 이용한 문법이 있습니다.   

하지만, 실무에서는 특별한 경우가 아니면, 거의 사용하지 않습니다.  
따라서, 이 블로그에서 다루기 보다는 [점프 투 자바](https://wikidocs.net/263){:target="_blank"} 블로그의 내용을 링크를 붙입니다.   


### 1
switch/case를 이용한 조건 분기를 자바에서 잘 사용하지 않는 이유는 조건에 **정수**만 사용할 수 있고, **break**문을 써야 하기 때문입니다. 코딩 중에 종종 break 문을 빠뜨려서 프로그램이 제대로 작동하지 않는 경우도 있고, 조건이 항상 정수(Integer)로만 되는 경우도 잘 없어서, 거의 사용하지 않습니다.   

### 2

그리고 굳이 switch/case 문 없이도 if... else if... else 구문으로도 충분히 코드를 작성할 수 있기 때문에 switch/case 구문 자체를 지원하지 않는 언어들도 있다고 합니다. 대표적으로 파이썬은 switch/case문이 없답니다.
