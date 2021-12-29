# Linux 伺服器建置_4_Neo4j資料庫伺服器
- [Neo4j: Graph Data Platform | Graph Database Management ](https://neo4j.com/)
- [Neo4j documentation](https://neo4j.com/docs/)



## [neo4j@dockerhub](https://hub.docker.com/_/neo4j)
- docker pull neo4j
```
docker run \
    --publish=7474:7474 --publish=7687:7687 \
    --volume=$HOME/neo4j/data:/data \
    neo4j
```
