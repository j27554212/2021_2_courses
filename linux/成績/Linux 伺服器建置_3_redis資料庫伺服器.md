# Linux 伺服器建置_3_redis資料庫伺服器

- [Docker學習筆記](https://peihsinsu.gitbooks.io/docker-note-book/content/)
- [Docker--从入门到实践](https://yeasy.gitbook.io/docker_practice/introduction)
- [Docker 教程](https://www.runoob.com/docker/docker-tutorial.html)

## [redis@dockerHUB](https://hub.docker.com/_/redis)
- [使用 Docker 安裝 Redis](https://marcus116.blogspot.com/2019/02/how-to-run-redis-in-docker.html)
- docker pull redis
- docker run -itd --name redis-test -p 6379:6379 redis
- docker exec -it redis-test /bin/bash

```
docker exec -it e819 bash
root@e819ea3d7a7b:/data# redis-cli
127.0.0.1:6379> ping
PONG
 
127.0.0.1:6379> set test "hello world"
OK
127.0.0.1:6379> get test
"hello world"
```

## [docker安裝redis設定密碼並連線的操作](https://www.796t.com/article.php?id=173205)
```
、在docker 倉庫下載redis

1
#在docker倉庫搜尋redis
2
docker search redis
3
#下載redis到本地倉庫不加版本號預設是最新版
4
docker pull redis
5
#檢視下載好的容器
6
docker images
2、用docker建立執行redis映象，並設定redis密碼

1
#使用docker run建立並啟動容器
2
#--requirepass 設定連線redis的密碼
3
docker run -p 6379:6379 --name redis -d redis:latest --requirepass "123456"
4
#檢視容器是否已經啟動
5
docker ps
3、本地方式連線redis

1
#本地連線直接使用bash命令 設定了密碼 用-a加密碼方式訪問
2
[root@apg-server ~]# docker exec -it redis redis-cli -a 123456
3
Warning: Using a password with '-a' or '-u' option on the command line interface may not be safe.
4
#set一個key測試
5
127.0.0.1:6379> set name xiaomianyang
6
OK
7
#查詢該key
8
127.0.0.1:6379> get name
9
"xiaomianyang"
4、檢視redis容器ip地址

1
[root@apg-server ~]# docker inspect redis | grep IPAddress
2
      "SecondaryIPAddresses": null,"IPAddress": "172.17.0.4",
5、遠端方式連線redis

view sourceprint?
1
#如果是在本機的話用localhost，如果是在其他地方用宿主機ip
2
[root@apg-server ~]# docker exec -it redis redis-cli -h localhost -p 6379 -a 123456
3
Warning: Using a password with '-a' or '-u' option on the command line interface may not be safe.
4
localhost:6379> get name
5
"xiaomianyang"

```
