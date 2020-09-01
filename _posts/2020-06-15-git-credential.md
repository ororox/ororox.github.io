---
title: git password 변경
tags:
- git
categories:
- Git
---

Git 사용중에 credential을 이용하여 비밀번호를 저장했는데, 비밀번호를 처음에 잘못 입력하면, 아래와 같은 에러가 발생하면서 push가 되지 않는다.

```
>> git push
remote: Invalid username or password.
fatal: Authentication failed for ...
```

이때는 credential을 unset 해서 지운 후 다시 사용하도록 설정하면 된다.

#### git credential 삭제

```
git config --unset credential.helper
```

#### git credential 설정

```
git config credential.helper store
```

#### 모든 프로젝트에 적용
--global 옵션을 주면 모든 git에 적용되지만, 나는 이렇게 잘 사용하진 않는다. (프로젝트 마다 할당한다)   
```
git config credential.helper store --global
```
