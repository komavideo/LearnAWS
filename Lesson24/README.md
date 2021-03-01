高可用性设计 - 建立新的子网区
=========================

## 知识点

* 建立新的可用区子网
* 在新的子网区添加 web-ec2 实例

## 实战演习

> 看图说话

## 操作内容

* 建立新的可用区子网
  + Name: deeplearnaws-web-1c
  + 配置路由表
* 在新的子网区添加 web-ec2 实例
  + Name: deeplearnaws-web2

### 修改 web2 服务内容

```bash
$ docker exec -it deeplearnaws-web sh
>root $ vi app.js
...
$ docker container restart deeplearnaws-web
```

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
