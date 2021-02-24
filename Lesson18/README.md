部署一个DB应用 - 还不行，还差一步设置
=================================

## 知识点

* 在公开网络中建立NAT网关
* 建立DB私有网络的路由表, 设置NAT网关
* 建立DB私有网络的安全组, 开放 3306 - MySQL端口

## 实战演习

> 看图说话

### NAT网关

+ Name: deeplearnaws-web-nat
+ SubNet: deeplearnaws-web-1a
+ Elastic IP

### 路由表

+ Name: deeplearnaws-db-rtb
+ Target: deeplearnaws-web-nat -> 0.0.0.0/0

### 安全组

+ Name: deeplearnaws-db-sg
+ Port: 3306

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
