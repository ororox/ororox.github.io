---
title: Git 필수 명령어 모음
categories:
- Git
tags:
- git
---

내가 필요해서 요약한 명령어 모음

**-- global**이 없으면, 해당 프로젝트에서의 설정

git config list

```config
git config --list
git config --global --list
```

git config 설정
```config
git config user.name "홍길동"
git config user.email "support@webisfree.com"

git config --global user.name "홍길동"
git config --global user.email "support@webisfree.com"
```

git config 삭제
```config
git config --unset user.name
git config --unset user.email

git config --unset-all user.name
git config --unset-all user.email

git config --unset --global user.name
git config --unset --global user.email

git config --unset-all --global user.name
git config --unset-all --global user.email
```
