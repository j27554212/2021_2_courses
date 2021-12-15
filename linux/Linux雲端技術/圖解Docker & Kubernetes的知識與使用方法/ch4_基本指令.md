# docker 基本指令
- docker version
- docker ps -a
- docker run --name apa000ex1 -d httpd
- docker ps
- docker stop apa000ex1
- docker ps -a
- docker run --name apa000ex2 -d -p 8080:80 httpd
- docker stop apa000ex2
- docker rm apa000ex2

- docker ps -a
- docker run --name apa000ex3 -d -p 8081:80 httpd
- docker run --name apa000ex4 -d -p 8082:80 httpd
- docker run --name apa000ex5 -d -p 8083:80 httpd
- docker ps
- docker stop apa000ex3
- docker stop apa000ex4
- docker stop apa000ex5
- docker rm apa000ex3
- docker rm apa000ex4
- docker rm apa000ex5

- docker run --name nginx000ex6 -d -p 8084:80 nginx


- docker ps
- docker stop nginx000ex6
- docker rm nginx000ex6


## MYSQL
- docker run --name mysql000ex7 -dit -e MYSQL_ROOT_PASSWORD=myrootpass mysql

- docker rm mysql000ex7
- docker ps -a
- docker image ls
- docker image rm httpd
- docker image ls
- docker image rm nginx mysql
- docker image ls


