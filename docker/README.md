# docker
linux에서 docker & docker-compose 설치
```
curl -fsSL https://get.docker.com/ | sudo sh
sudo usermod -aG docker $USER

sudo curl -L "https://github.com/docker/compose/releases/download/1.24.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose

# check (re-login)
docker version
docker-compose version

# reboot
sudo reboot
```

기본적인 명령어 형태
```script
$ docker run -d \
-p 8888:8888 \
-e DB_PASSWORD=1234 \
kangthink/docker-sample:latest
```
## 로그
docker의 로그를 보고 싶을 때

### 로그를 볼 때
```
$ docker logs [OPTIONS] CONTAINER
 ```

#### 새로 생성되는 로그를 관찰할 때
```
$ docker logs -f CONTAINER
 ```

## 이미지
이미지를 만들거나 삭제하거나 관찰할 때

### 이미지를 삭제
```
$ docker rmi [OPTIONS] IMAGE [IMAGE...]
```
