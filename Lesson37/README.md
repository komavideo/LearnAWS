连接MySQL - phpMyAdmin管理工具
=============================

## 知识点

* 使用 phpMyAdmin 管理工具连接 MySQL 数据库实例

## phpMyAdmin官网

https://www.phpmyadmin.net/

### Docker.Hub

https://hub.docker.com/r/phpmyadmin/phpmyadmin/

## 实战演习

### docker-compose.yml

```yml
version: '3' 
services:
  phpmyadmin:
    image: phpmyadmin:latest
    container_name: web_phpmyadmin
    ports:
      - 80:80
    environment:
      - PMA_HOST=mysqldev.cbcbjcjywvwn.ap-northeast-1.rds.amazonaws.com
      - PMA_USER=root
      - PMA_PASSWORD=12345678
```

```bash
# 编译服务
$ sudo docker-compose build
# 容器启动(精灵线程)
$ sudo docker-compose up -d
# 查询容器状态
$ sudo docker-compose ps
```

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS