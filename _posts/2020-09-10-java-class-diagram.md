---
title: 클래스 다이어그램, Class Diagram
categories:
- Java Training
tags:
- 자바연습
---

클래스 다이어그램은 주로 UML(Unified Modeling Language)이라는 형태로 그립니다.

UML은 프로그램 언어를 모르는 사람도 쉽게 이해할 수 있고, 다른 프로그램 언어에서도 공통으로 사용할 수 있도록 만든 언어라는 뜻입니다.   

하지만, 역시나 현실에서는 프로그램을 모르는 사람은 UML의 뜻을 제대로 이해할 수 없고, 다른 프로그램 언어에서도 공통으로 사용하기에는 무리가 있는 표현 방식입니다.

UML은 자바에서는 꽤 유용하게 사용할 수 있지만, 그 역시도 처음 프로그램을 배울 때 유용하고, 실무에는 이런 것까지 그리면서 프로그램을 만들 여유가 없습니다. 하지만, 우리는 배우는 중이므로 의사소통에 꽤나 유용합니다.

클래스 다이어그램에 대한 내용은 일일이 다 적으면 내용이 많으므로, 아래에 좋은 블로그를 링크해 두었습니다. 한 번 쓱~ 읽어보시면 좋습니다.

[UML 클래스 다이어그램 작성법](https://gmlwjd9405.github.io/2018/07/04/class-diagram.html){:target="_blank"}

### Book Class

도서관이니까 책이 필요하겠지요? 책에 필요한 요소가 무엇이 있을까요? 그리고, 판매용 책이 아닌 도서관에 있는 책으로서 필요한 요소가 무엇일까요?   
사람에 따라 여러 가지 의견이 있을 수 있고, 고객의 **요구사항**에 따라 또한 다를 것입니다. 그런 걸 결정하고, 개발자에게 개발을 맡기는 사람을 **설계자**라고 합니다. 설계자의 입장에서 저는 아래와 같은 **상태**요소가 필요할 것 같습니다.   

- ISBN   
- 제목   
- 저자   
- 페이지수   
- 대출상태(Y: 대출중/N: 입고)

또한, 대출상태를 변경하는 **함수**도 필요할 것 같습니다.

- 대출( )

### 클래스 다이어그램

위에서 말한 내용을 참고하여 UML을 이용한 클래스 다이어그램을 아래와 같이 그릴 수 있습니다.

<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" width="161px" viewBox="-0.5 -0.5 161 171" content="&lt;mxfile host=&quot;app.diagrams.net&quot; modified=&quot;2020-09-29T23:56:38.544Z&quot; agent=&quot;5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.121 Safari/537.36&quot; etag=&quot;3z9NDy5jVPqEis5dL0J4&quot; version=&quot;13.7.6&quot;&gt;&lt;diagram id=&quot;C5RBs43oDa-KdzZeNtuy&quot; name=&quot;Page-1&quot;&gt;7VddT9swFP01lbYHpny0pXtsAmOMgoDS8ewmbmLVsTPnljb8+l0nTtKQDui0qhKaVCHf4+vr3HOOg9Nz/WRzoUgaX8uQ8p5jhZuee9ZznNFwhH81kJdAf+SUQKRYWEJ2A0zZMzWgZdAVC2nWSgQpObC0DQZSCBpACyNKyXU7bSF5e9eURLQDTAPCu+gjCyE2bTmnDf6dsiiudraHX8uZhFTJppMsJqFcb0Huec/1lZRQjpKNT7nmruLl8TJ/5JPl8OLHXfaLzLyrh5ufJ2Wxb/ssqVtQVMBflz4n4nl8NXevs7vLWTQb3EW5MkusJ8JXhi9PyqXpF/KKxGzNEk4ERt5CCpiaGaTAI5xFAscBPhtVCDxRBQz5H5sJkCmiQcx4OCG5XOkOMiDBsoq8WCr2jGUJxykbAZxWYKzkDFsZU70SYQtRRTPMua1osWtoQjIwOYHknKQZmxcPrFMSoiImPAkgk6qQXImQhiaqdS4CUHJZO0evf6cYRjTNBt1sWdGIc0FlQkHlmGJma5+Zg2ZX8bqxrT00WLxt2VMDEnNUorp2vd09Hi0iIiSh2c99sV//nfuhIq3tCEfhBQHqaRqzbRPiYKvVBiqsuYdN7Y5NTzC8nHo3PXeMoykoJqKObZF52LIopwv4o0GzlARYY1LknPUb5N50riGJaxe8MEfMwpCKwjxAgJT+0o5JJRNQUDPw8IcE+taXQW+AD+RjbDcx/nS6Al8K9BlhhaEomndNtYF3WO3VQ/y21fK2gvsqvW2slsT76uns1BMYaBbHH1TNV94yMSTcDA+l+cA5subuTs3JCuKb5EOf4uPqfjo6su79nbrre5ePxEApvSbtv+7/Unfb6h9Z+EFH+I7EnBV3SkOHvfO+9Yb+CSqpy1WCP2g/nJ3YHVO4XVO4OwzAyZzyW5kxYFLXV2XuC2Mc6z+37b7zkjY6kKjDHaJit9Zc6m+1T59x+KFf5ocT9nDvaQybr9TySt586rvnvwE=&lt;/diagram&gt;&lt;/mxfile&gt;" onclick="(function(svg){var src=window.event.target||window.event.srcElement;while (src!=null&amp;&amp;src.nodeName.toLowerCase()!='a'){src=src.parentNode;}if(src==null){if(svg.wnd!=null&amp;&amp;!svg.wnd.closed){svg.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&amp;&amp;evt.source==svg.wnd){svg.wnd.postMessage(decodeURIComponent(svg.getAttribute('content')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);svg.wnd=window.open('https://viewer.diagrams.net/?client=1&amp;edit=_blank');}}})(this);" style="cursor:pointer;max-width:100%;max-height:171px;"><defs><clipPath id="mx-clip-4-31-152-26-0"><rect x="4" y="31" width="152" height="26"/></clipPath><clipPath id="mx-clip-4-57-152-26-0"><rect x="4" y="57" width="152" height="26"/></clipPath><clipPath id="mx-clip-4-83-152-26-0"><rect x="4" y="83" width="152" height="26"/></clipPath><clipPath id="mx-clip-4-109-152-26-0"><rect x="4" y="109" width="152" height="26"/></clipPath><clipPath id="mx-clip-4-143-152-26-0"><rect x="4" y="143" width="152" height="26"/></clipPath></defs><g><path d="M 0 26 L 0 0 L 160 0 L 160 26" fill="#ffffff" stroke="#000000" stroke-miterlimit="10" pointer-events="all"/><path d="M 0 26 L 0 170 L 160 170 L 160 26" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><path d="M 0 26 L 160 26" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g fill="#000000" font-family="Helvetica" font-style="italic" pointer-events="none" text-anchor="middle" font-size="12px"><text x="79.5" y="17.5">Book</text></g><g fill="#000000" font-family="Helvetica" pointer-events="none" clip-path="url(#mx-clip-4-31-152-26-0)" font-size="12px"><text x="5.5" y="43.5">- ISBN: String</text></g><g fill="#000000" font-family="Helvetica" pointer-events="none" clip-path="url(#mx-clip-4-57-152-26-0)" font-size="12px"><text x="5.5" y="69.5">- title:String</text></g><g fill="#000000" font-family="Helvetica" pointer-events="none" clip-path="url(#mx-clip-4-83-152-26-0)" font-size="12px"><text x="5.5" y="95.5">- authNm: String</text></g><g fill="#000000" font-family="Helvetica" pointer-events="none" clip-path="url(#mx-clip-4-109-152-26-0)" font-size="12px"><text x="5.5" y="121.5">- pageCount: int</text></g><path d="M 0 134 L 160 134" fill="none" stroke="#000000" stroke-miterlimit="10" pointer-events="none"/><g fill="#000000" font-family="Helvetica" pointer-events="none" clip-path="url(#mx-clip-4-143-152-26-0)" font-size="12px"><text x="5.5" y="155.5">+ borrow() : String</text></g></g></svg>

### Book 클래스 코딩

위에서 그린 UML을 참고로 하여, 아래와 같은 자바 클래스 코딩이 가능합니다.   
단, 아직 borrow 메소드에 대한 정의가 부족하므로, TODO 코멘트로 남길 수 밖에 없고, 이후에 추가 개발이 필요한 상태로 남겨 둡니다.   

```java
public class Book {
	
	private String ISBN;
	private int page;
	private String title;
	private String authNm;
	
	public void borrow(String yn) {
		//TODO: 대출 서비스
	}
}
```   

원래 설계서에서는 메소드에 대한 자세한 기술이 있어야 프로그래밍이 가능하며, 때로는 문서로 때로는 구두로 해당 기능을 알려주기도 합니다. 다만, 이번 포스팅에서는 UML을 이용하여 클래스를 개발할 수 있다는 예시를 보여주는 것으로 합니다.
