建立公私网 - 公私分明才能网络安全
=============================

## 知识点

* 建立公有网段
* 建立私有网段

## 官网

https://docs.aws.amazon.com/zh_cn/vpc/latest/userguide/working-with-vpcs.html

## 实战演习

### 子网所属VPC

+ deeplearnaws-vpc

### 公开网络

主要用于对外公开的服务器，如：Web，API服务器

+ 网段决定
  + 172.16.10.0/24
  + ap-northeast-1a
+ 标签
  * Name:deeplearnaws-web-1a

### 私有网络

主要用于内部使用的服务器，如：DB, Redis等

+ 网段决定
  + 172.16.20.0/24
  + ap-northeast-1a
+ 标签
  * Name:deeplearnaws-db-1a

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
