# 5주차 - Docker

## 오늘 배운 내용

- Docker 이해하기
- Docker 명령어와 컨테이너 실습
- GitHub Issue로 실습 관리하기

## 새로 배운 명령어
```docker
docker run
docker ps
docker rm
docker images
docker logs <컨테이너 이름>
docker stop
docker start
docker restart
docker exec
```

## curl 확인 결과

### nginx1
```text
$ curl localhost:8091
<h1>Welcome to nginx1</h1>
```
###nginx2
```text
$ curl localhost:8092
<h1>Welcome to nginx2</h1>
```
###nginx3
```text
$ curl localhost:8091
<h1>Welcome to nginx3</h1>
```

