# 常用命令

1. 启动`kafka`

   > `./bin/kafka-server-start.sh  ../config/server.properties`

   - 后台启动

     > `./bin/kafka-server-start.sh -daemon ../config/server.properties`

2. 新建topic

   > `bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic topic名称`

3. 查看topic

4. 