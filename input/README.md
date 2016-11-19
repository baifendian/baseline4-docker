## 部署数据探头

### 部署 Nginx
1. 修改nginx配置文件
1. 启动容器
```
Docker Run Command
```

### 部署MongoDB
1. Version: 3.0.14, Dockerfile: [3.0.14](https://github.com/docker-library/mongo/blob/b37a4891feffeafb77febd2833d96b59cf28d6a8/3.0/Dockerfile)
1. 启动容器
```
docker run -d --net=host --name=bfd-mongo docker.baifendian.com/sys/mongo:3.0.14
```
1. 使用`docker logs bfd-mongo`查看日志，待mongodb启动完成后使用admin验证服务是否正确启动
```
>docker exec -it bfd-mongo mongo admin
MongoDB shell version: 3.0.14
connecting to: admin
Welcome to the MongoDB shell.
For interactive help, type "help".
For more comprehensive documentation, see
	http://docs.mongodb.org/
Questions? Try the support group
	http://groups.google.com/group/mongodb-user
>
>
```

### 部署 dataProcessService
### 部署 webService
### 部署 input_web
