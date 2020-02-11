# linux

## user
```
# user 추가
$ sudo adduser USERNAME

# user 목록
$ sudo vi /etc/passwd

# user 삭제
$ sudo userdel USERNAME

# user pw 변경
sudo passwd USERNAME
```

## group
```
# group 추가
$ sudo groupadd GROUPNAME

# group 삭제
$ sudo groupdel GROUPNAME

# user를 그룹에 추가
$ sudo adduser USERNAME GROUPNAME

# user를 그룹에서 제외
$ sudo deluser USERNAME GROUPNAME

# group 목록
$ sudo vi /etc/group
```

## permission
777 (owner group etc)  
4 = read  
2 = write  
1 = execute  

```
# 해당 파일 혹은 폴더 및 아래 모두 권한
$ sudo chmod 777 FILE -R
```

## ownership
```
$ sudo chown -R USER FILE
```
