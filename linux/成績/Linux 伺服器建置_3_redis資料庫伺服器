# Linux 伺服器建置_3_redis資料庫伺服器

- [Docker學習筆記](https://peihsinsu.gitbooks.io/docker-note-book/content/)

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

