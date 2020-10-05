---
title: Java Training Tools
categories:
- Tools
tags:
- java
- jdk
- eclipse
---

**Java-training.zip** 파일은 자바 개발에 필요한 도구를 한 곳에 모아서 **압축파일**로 만든 것입니다.    

### 소개

기존에는 Java를 설치하고, eclipse를 설치하고, workspace를 설정하는 번거로운 작업으로 안내했으나, 이제는 <span style="color:red"><b>설치가 필요 없는 압축 파일</b></span>을 "C:\ 드라이브"에 압축을 풀어놓기만 하면 됩니다.

반드시 <span style="color:red"><b>C:\ 드라이브</b></span>에 압축을 풀어야 정상작동 합니다.   
(D:\ 드라이브에 압축해제 할 경우 추가 설정 필요)

[Java Training Tools](https://github.com/ororox/java-training-tools/blob/master/Java-training.zip){:target="_blank" rel="noopener"}

![Java Training Tools Download]({{ 'assets/images/post/java-training-download.png' | relative_url }})

링크 이동 후 "Download" 버튼 클릭 후 잠시 기다리면 다운로드가 시작됩니다. (환경에 따라 오래 걸리는 경우도 있음).  다운로드 받은 "Java-training.zip" 파일을 아래와 같이 "C:\Java-training"에 압축을 풀어 배치합니다.

![java-training]({{ 'assets/images/post/java-training.png' | relative_url }})

**이클립스 링크를 더블클릭**하면, 이클립스가 실행되고, 해당 아이콘을 **바탕화면에 Drag&Drop**으로 가져다 두어도 됩니다.


### 구동테스트

C:\ 드라이브에 압축해제 후 이클립스 구동을 확인합니다.

반드시 <span style="color:red"><b>C:\ 드라이브</b></span>에 압축을 풀어야 정상작동 합니다.

> C:\Java-training   

폴더 안에 있는 보라색 이클립스 아이콘을 더블클릭하면, 프로그램이 실행됩니다.

![splash]({{ 'assets/images/post/splash.png' | relative_url }})


이클립스가 완전히 구동되면, 아래와 같은 화면이 보이며, 화면 상단에 있는 초록색 Run 버튼을 누르면, 화면 중간에 있는 소스코드가 실행됩니다.

![java-test]({{ 'assets/images/post/java-test.png' | relative_url }})

아래쪽 Console 창에 "Hello World!"가 보이면, 정상작동된 것 입니다.   
>"Hello World!"


### 구성요소

Java Training Tools는 간단하게 2개의 구성요소로 이루어져 있습니다.

* Eclipse IDE 2020‑06
* Open JDK 14.0.1   


#### 이클립스(Eclipse)

이클립스는 자바 개발자가 가장 많이 사용하는 IDE 툴입니다.
[이클립스, 개발자의 워드프로세서](https://ororox.tistory.com/2)

IDE는 개발에 필요한 통합환경을 제공하는 **프로그램을 만드는 프로그램**이라고 볼 수 있습니다. 이클립스는 태생부터 자바로 구현되어 있고, 무료로 배포되고 있어서 예전부터 많이 사용하던 프로그램입니다.

>이클립스는 혼자서 구동하는 프로그램이 아닙니다.

흔히 **플랫폼** 개발툴이라고도 하는데, 개발자의 필요에 따라 기존에 만들어진 개발툴을 추가, 삭제, 편집할 수 있을 뿐만 아니라 스스로 제작툴을 만들어 추가할 수도 있습니다. 이클립스 실행을 위해서는 반드시 외부에 **JDK**가 있어야 실행됩니다. 이클립스는 javaw로 구동되는 의존성이 있는 프로그램입니다.

이클립스는 여러 가지 버전이 있는데, 폴더에 포함된 이클립스는 "IDE 2020‑06" 버전을 기본으로 로딩화면만 일부 커스텀하였습니다.

#### Open JDK
통상 Oracle Java Development Kit (Oracle JDK)를 설치하지만, 오라클이 자바 라이센스 유료화를 선언했기에 (사실 제가 하는 강의에서 라이센스 문제가 발생할 여지는 없지만), Open JDK를 사용하였습니다.  둘 간의 차이는 거의 없고, 프로그램을 처음 접하는 초보자는 둘 간의 차이를 전혀 느낄 수 없기에 이번 툴은 Open JDK를 자바 표준개발 도구로 사용하였습니다.


### 폴더설명

압축 파일을 풀면 총 3개의 폴더를 확인할 수 있습니다.

**eclipse**   
이클립스 실행 파일이 있는 곳이고, "Java-training" 폴더에 있던 아이콘은 여기에 있는 실행 파일의 바로가기입니다. 따라서 그냥 "eclipse" 폴더에 있는 "eclipse" 파일을 실행해도 됩니다.

**jdk-14.0.1**   
Open JDK 14.0.1 버전의 자바 개발도구가 들어있습니다. "C:\Java-training\jdk-14.0.1\bin" 폴더 아래에서 **java, javac, javadoc, javap, javaw** 등의 프로그램을 확인할 수 있습니다.

**workspace**   
폴더는 이클립스에서 만드는 작성하는 소스 코드와 컴파일 코드가 저장되는 저장소 폴더입니다. 처음에는 비어있지만, 프로그램을 개발할수록 이곳에 소스 코드와 컴파일된 실행 파일이 저장됩니다. 원래는 이클립스 실행 시에 선택하게 되어 있지만, 초보자의 번거로움을 피하고자 제가 임의로 설정한 저장소입니다.


### 만드는 방법
Java-training.zip 파일은 아래와 같은 과정으로 만들었습니다.

**내용이 잘 이해되지 않으면 굳이 읽지 않아도 됩니다.**

제가 만든 툴과 비슷하게 만들고 싶은 사람들을 위한 일종의 **제작 가이드**입니다.

보통 자바는 설치를 기본적으로 합니다. JDK를 설치하고, 윈도우 환경변수에서 "PATH"를 설정하고, ... 
하여튼... 복잡한 절차가 필요합니다. 자바를 처음 접한 사람에게는 이런 절차마저도 부담스럽습니다.

실무에서도 동시에 프로젝트가 여러 개 관리해야 할 경우, 프로젝트 간의 툴 의존성을 없애기 위해 하나의 폴더에 모든 툴을 제공하는 경우가 늘어나고 있습니다.


적당한 폴더를 하나 만듭니다.   
> C:\Java-training

해당 폴더 아래에 JDK 압축파일을 풀어둡니다. 중요한 것은 **설치가 아니라 압축을 풀기**만 한다는 겁니다. JDK는 설치파일도 있지만, zip과 같은 형태의 압축파일도 제공합니다. 방금 만든 폴더 아래에 압축파일을 풀어둡니다. 버전을 구분하기 위해서 폴더명에 버전을 붙이기도 하고, 그냥 "jdk"로 해도 무방한데, 저는 버전을 같이 붙여서 만들었습니다.   
> C:\Java-training\jdk-14.0.1

이클립스도 설치가 아닌 압축파일을 받아서 폴더 아래에 풀어둡니다.   
> C:\Java-training\eclipse

<span style="color:red"><b>여기서부터 중요</b></span>   
**C:\Java-training\eclipse** 폴더에 "eclipse.ini" 파일에 아래 내용을 추가해야 합니다.

```
-vm
../jdk-14.0.1/bin/javaw.exe
```

"openFile"과 "-vmargs" 사이에 추가하고,

```
openFile
--launcher.appendVmargs
// 여기에 추가
-vmargs
-Dosgi.requiredJavaVersion=1.8
```

최종 모양은 이렇게 됩니다.   

```
openFile
--launcher.appendVmargs
-vm
../jdk-14.0.1/bin/javaw.exe
-vmargs
-Dosgi.requiredJavaVersion=1.8
```

"javaw.exe"는 java랑 같은 실행 파일이지만, 콘솔 없이 실행되는 파일이라고 합니다.
>"../jdk-14.0.1/bin/"
이 구문이 적용되기 위해서는 반드시 JDK와 이클립스가 동일한 폴더에 동일한 레벨에 있어야 합니다. 다른 레벨에 폴더를 만들었으면, 구문을 다르게 변경해야 합니다.

이후에 이클립스를 실행하고, 워크스페이스 경로를 아래와 같이 설정한 후 종료하면,
> C:\Java-training\eclipse   
> C:\Java-training\jdk-14.0.1   
> C:\Java-training\workspace

![java training tool]({{ 'assets/images/post/java-training.png' | relative_url }})

위와 같은 폴더 구조가 되고,      
이후에 이클립스 "바로가기" 아이콘을 배치하면 끝.

"D:\ " 드라이드로 옮겨서 실행하려면, 위에서 설정한 파일을 참고해서 D:\로 이동가능 합니다.

### 강의동영상(유튜브)

아래 그림을 클릭하면, 유튜브로 이동합니다.

[![Java training tools](https://i9.ytimg.com/vi/9U5_Phuk0g0/mq1.jpg?sqp=CKi27PsF&rs=AOn4CLDZ9CA4O_2MmPRjca4yKNCnsqBoXg)](https://youtu.be/9U5_Phuk0g0)
