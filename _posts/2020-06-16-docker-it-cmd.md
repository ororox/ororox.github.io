---
title: 도커(Docker) 명령어 모음
categories:
- Docker
tags:
- docker
---

내가 필요해서 요약한 도커 명령어 모음

### 프로세스 확인
```
$ docker ps -a
```

### 도커 내부로 들어가기
CONTAINER ID 혹은 NAMES로 들어간다.   

```
$ docker exec -it [134adb2ba12 혹은 my-container] /bin/bash
```

### 도커에서 나오기
exit

```
# exit
$ 
```

### 도커 시작, 재시작, 중지

```
$ docker start [134adb2ba12 혹은 my-container]
$ docker restart [134adb2ba12 혹은 my-container]
$ docker stop [134adb2ba12 혹은 my-container]
```
