# 说明 

Mac

```
docker run \
    --publish=7474:7474 --publish=7687:7687 \
    --volume=$HOME/Desktop/neo4j/data:/data \
    neo4j
```

data数据持久化的目录: ```/Desktop/neo4j/data```

Ubuntu

```
docker run \
    --name testneo4j \
    -p7474:7474 -p7687:7687 \
    -d \
    -v $HOME/neo4j/data:/data \
    -v $HOME/neo4j/logs:/logs \
    -v $HOME/neo4j/import:/var/lib/neo4j/import \
    -v $HOME/neo4j/plugins:/plugins \
    --env NEO4J_AUTH=neo4j/test \
    neo4j:latest
```

注意 : 这里的登录密码已经定义好是test

数据持久化的路径 :


```
# 说明，echo $HOME 输出， root
# 数据路径
/root/neo4j/
```

参考资料 :

[https://neo4j.com/developer/docker-run-neo4j/](https://neo4j.com/developer/docker-run-neo4j/)
