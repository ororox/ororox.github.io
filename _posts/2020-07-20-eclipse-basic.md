---
title: 이클립스 용어설명
categories:
- Java Beginner Course
tags:
- eclipse
---

이클립스는 자바 개발자들이 가장 애용하는 개발툴입니다.

[이클립스, 개발자의 워드프로세서](../../칼럼/eclipse/){:target="_blank"}를 참조할 수 있습니다.

이클립스는 프로그램 코드를 편집하는 편집창과 개발중인 프로그램을 실행할 때 상태를 보기 위한 콘솔, 프로그램의 구조를 보기 위한 Outline 등을 다양한 화면을 한곳에서 볼 수 있게 모아놓은 **플랫폼 형태**의 프로그램 입니다. 이렇게 작은 프로그램을 **플러그인**이라고 합니다.

### View
이클립스 화면 보이는 Package Explore, Outline, Console, Problems와 소스코드를 편집하는 편집창을 각각 "뷰(view)"라고 부릅니다. 이런 뷰는 필요에 따라 추가하거나 안보이게 닫아 둘 수 있습니다. 이러한 View는 대부분 **플러그인**으로 구성되어 있습니다. 하나의 플러그인이 하나의 View를 구성하기도 하고, 여러 개의 플러그인 프로그램이 하나의 View를 위해 필요하기도 합니다.

![view]({{ 'assets/images/post/view.png' | relative_url }})

메뉴에서 **Window > Show View**를 따라가면, 현재 사용할 수 있는 다양한 View를 볼 수 있습니다. 가장 하단에 "Other..."를 선택하시면, 폴더별로 정리된 많은 View를 발견하실 수 있을 겁니다. 이 중에서 필요한 것만 골라서 선택해서 사용합니다.


### Perspective
퍼스펙티브는 "관점"이라는 뜻이 있습니다. 이클립스에는 너무도 많은 "뷰(View)"가 있습니다. 그래서 뭘 사용해야 할지 망설여집니다. 이때, Perspective는 사용자의 "관점"에 따라서 필요한 이클립스 뷰를 어느 정도 모아둔 것입니다. 즉, 개발용, 테스트용, 버전관리용으로 대략적을 필요한 View를 모아두었습니다. 반드시 모든 사용자가 그러한 것은 아니지만, 대략 비슷하게 사용합니다.

보통은 Perspective를 하나 선택하고, 불필요한 view는 닫고, 필요한 view는 추가해서 나만의 개발환경을 만들어서 사용합니다.

Perspective는 맨 우측 상단의 작은 아이콘을 선택하거나, 메뉴에서  **Window > Perspective > Open Perspective**에서 선택하여 사용합니다.   

![perspective]({{ 'assets/images/post/perspective.png' | relative_url }})

사용중에 조작을 실수하거나 잘못클릭하여 창을 닫았거나 했는데, 뭘 열고 닫았는지 헷갈리는 경우에는 메뉴에서  **Window > Perspective > Reset Perspective..** 기능을 이용해서 초기화하기도 합니다.

### Workspace
워크스페이스는 소스코드가 저장되는 폴더를 말합니다. 개발자의 성향이나 프로젝트의 성향에 따라 이클립스 프로그램과 같은 폴더에 만들기도 하고, 아예 다른 드라이브에 만들기도 합니다.

예전에는 C:\ 드라이브에 이클립스 실행프로그램을 설치하고, D:\ 드라이브에 워크스페이스를 설정하곤 했습니다. 혹시라도 PC에 문제가 생기면, C:\ 드라이브를 포맷하더라도 소스코드는 D:\ 드라이브에 있으니 개발한 내용을 보존할 수 있었습니다.

최근에는 Git, SVN 등을 통해서 소스코드를 아예 다른 곳(서버 등)에 보관하기 때문에 워크스페이스가 C에 있던 D에 있던 신경쓰지 않는 경향이 있습니다. 그래서 여러 개의 프로젝트를 동시에 진행하는 경우에는 프로젝트 단위별로 하나의 폴더에 이클립스 실행파일과 소스코드를 동시에 가지고 다니기도 합니다.
