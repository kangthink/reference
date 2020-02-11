# docker

기본적인 명령어 형태
```script
$ docker run -d \
-p 8888:8888 \
-e DB_PASSWORD=1234 \
kangthink/docker-sample:latest
```

### 로그를 볼 때
```
$ docker logs [OPTIONS] CONTAINER
 ```

#### 새로 생성되는 로그를 관찰할 때
```
$ docker logs -f CONTAINER
 ```
