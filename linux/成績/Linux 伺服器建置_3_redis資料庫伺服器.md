# Linux 伺服器建置_3_redis資料庫伺服器

- [Docker學習筆記](https://peihsinsu.gitbooks.io/docker-note-book/content/)
- [Docker--从入门到实践](https://yeasy.gitbook.io/docker_practice/introduction)
- [Docker 教程](https://www.runoob.com/docker/docker-tutorial.html)

## [redis@dockerHUB](https://hub.docker.com/_/redis)
- [使用 Docker 安裝 Redis](https://marcus116.blogspot.com/2019/02/how-to-run-redis-in-docker.html)
- docker pull redis
```
Using default tag: latest
latest: Pulling from library/redis
a2abf6c4d29d: Pull complete 
c7a4e4382001: Pull complete 
4044b9ba67c9: Pull complete 
c8388a79482f: Pull complete 
413c8bb60be2: Pull complete 
1abfd3011519: Pull complete 
Digest: sha256:db485f2e245b5b3329fdc7eff4eb00f913e09d8feb9ca720788059fdc2ed8339
Status: Downloaded newer image for redis:latest
docker.io/library/redis:latest
```
- docker run -itd --name myredis -p 6379:6379 redis
```
2122bd6239f461779f13c9ee397ae12dc0338a781f5a10ba808ebf97e4b4fd61
docker: Error response from daemon: driver failed programming external connectivity on endpoint redis-test (fdb0421328f619581e1f985197989afb3cf7b7c0749830043d5d9a0f6007955e): Bind for 0.0.0.0:6379 failed: port is already allocated.
```
- docker exec -it myredis /bin/bash

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

## ACL
```
127.0.0.1:6379> acl --help
(error) ERR Unknown subcommand or wrong number of arguments for '--help'. Try ACL HELP.
127.0.0.1:6379> ACL HELP
 1) ACL <subcommand> [<arg> [value] [opt] ...]. Subcommands are:
 2) CAT [<category>]
 3)     List all commands that belong to <category>, or all command categories
 4)     when no category is specified.
 5) DELUSER <username> [<username> ...]
 6)     Delete a list of users.
 7) GETUSER <username>
 8)     Get the user's details.
 9) GENPASS [<bits>]
10)     Generate a secure 256-bit user password. The optional `bits` argument can
11)     be used to specify a different size.
12) LIST
13)     Show users details in config file format.
14) LOAD
15)     Reload users from the ACL file.
16) LOG [<count> | RESET]


127.0.0.1:6379> acl USERS
1) "default"

127.0.0.1:6379> acl LOG
(empty array)
127.0.0.1:6379> acl WHOAMI
"default"
127.0.0.1:6379> acl LIST
1) "user default on nopass ~* &* +@all"

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
