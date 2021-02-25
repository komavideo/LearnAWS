通过 Web 应用连接到 MySQL 数据库服务器
==================================

## 知识点

* 更新 Web 应用 Docker 版本
* 确认连接到数据库实例

## Web镜像(Docker Hub)

https://hub.docker.com/r/komavideo/deeplearnaws-web

## 实战演习

```bash
# 从DockerHub上获取deeplearnaws-web镜像
$ docker pull komavideo/deeplearnaws-web:latest
$ docker run --name deeplearnaws-web -p 80:3000 -d --restart=always komavideo/deeplearnaws-web:latest
$ docker container ls -a
$ docker logs -f deeplearnaws-web
$ docker container stop deeplearnaws-web
$ docker container rm deeplearnaws-web
$ docker ps
# 编辑调整
$ docker exec -it deeplearnaws-web sh
>root $ vi app.js
$ docker container restart deeplearnaws-web
```

## 打包Web-AMI

+ Name: deeplearnaws-web-ami

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
