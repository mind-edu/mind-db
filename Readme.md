# 说明 

一条命令直接就可以运行成功的

Mac

```
docker run \
    --publish=7474:7474 --publish=7687:7687 \
    --volume=$HOME/Desktop/neo4j/data:/data \
    neo4j
```

Ubuntu

```
docker run \
    --publish=7474:7474 --publish=7687:7687 \
    --volume=$HOME/neo4j/data:/data \
    neo4j
```

数据保存的路径：
```
/home/ubuntu/neo4j/data
```

[https://hub.docker.com/_/neo4j/](https://hub.docker.com/_/neo4j/)
