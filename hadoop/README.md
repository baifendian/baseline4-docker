## 部署Hadoop, 单节点模式

### 部署HDFS，Yarn
1. Dockerfile:[2.6.0](https://github.com/sequenceiq/hadoop-docker/blob/master/Dockerfile)
1. 启动

    ```
    docker run -d -p 50010:50010 -p 50020:50020 -p 50070:50070 \
    -p 50075:50075 -p 50090:50090 -p 8020:8020 -p 9000:9000 \
    -p 10020:10020 -p 19888:19888 -p 8030:8030 -p 8031:8031 \
    -p 8032:8032 -p 8033:8033 -p 8040:8040 -p 8042:8042 -p 8088:8088 \
    -p 49707:49707 -p 2122:2122 \
    docker.baifendian.com/baseline4/hadoop:2.6.0
    ```
