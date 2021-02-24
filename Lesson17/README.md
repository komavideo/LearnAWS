部署一个Web应用 - 建立Node.js+Docker的应用程序
==========================================

## 知识点

* 部署一个 Node.js 的 Web 应用
* 把应用通过 Docker(Hub) 方式进行部署
* 修改安全组，追加开放 80 端口

## 今后预定

+ 部署到 ECR + ECS

## 实战演习

> 图解说明

### Docker Hub

+ deeplearnaws-web

https://hub.docker.com/r/komavideo/deeplearnaws-web

### 修改安全组， 追加开放80端口

> 视频操作 - 开放 80 端口

### 操作步骤

```bash
# 从DockerHub上获取deeplearnaws-web镜像
$ docker pull komavideo/deeplearnaws-web:latest
$ docker run --name deeplearnaws-web -p 80:3000 -d komavideo/deeplearnaws-web:latest
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

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
