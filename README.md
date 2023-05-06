## docker-test

Dockerfile, images 만들고 container 실행시켜보기

실행한 커맨드

이미지 만들기

```
docker build -f Dockerfile -t fun-docker .
```

이미지 확인

```
 docker ps
```

만든 이미지 실행

```
docker run -d -p 8080:8080 fun-docker
```

docker hub에 푸시하기전 태그달기

```
docker tag fun-docker:latest minji2687/docker-example:latest
```

푸시하기

```
docker push minji2687/docker-example:latest
```
