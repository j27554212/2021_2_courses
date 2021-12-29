# Linux 伺服器建置_4_Neo4j資料庫伺服器
- [Neo4j: Graph Data Platform | Graph Database Management ](https://neo4j.com/)
- [Neo4j documentation](https://neo4j.com/docs/)
- [看圖說故事，讓 Neo4j 重新詮釋你的資料庫 ](https://ithelp.ithome.com.tw/users/20092912/ironman/3834)


## [neo4j@dockerhub](https://hub.docker.com/_/neo4j)
- docker pull neo4j
```
docker run \
    --publish=7474:7474 --publish=7687:7687 \
    --volume=$HOME/neo4j/data:/data \
    neo4j
```

## [以 Docker 執行 Neo4j 資料庫](https://ithelp.ithome.com.tw/articles/10250575)
```
docker run \
    --name egg_neo4j \
    -p7474:7474 -p7687:7687 \
    -d \
    -v $HOME/neo4j/data:/data \
    -v $HOME/neo4j/logs:/logs \
    -v $HOME/neo4j/import:/var/lib/neo4j/import \
    -v $HOME/neo4j/plugins:/plugins \
    --env NEO4J_AUTH=neo4j/mypassword \
    neo4j:latest
```
