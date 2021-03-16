MySQL@RDS - 准备工作
===================

## 知识点

* 建立RDS MySQL前的准备工作

## 实战演习

### VPC子网,安全组,DB子网组,参数组,选项组

+ VPC子网
  - Name: deeplearnaws-db-1c
  - CIDR: 172.16.21.0/24
+ 安全组
  - Name: deeplearnaws-db-sg <- 可以直接使用，但生产环境时应只保留3306端口
+ DB子网组
  - Name: deeplearnaws-db-subnet-group
+ 参数组
  - Name: deeplearnaws-db-parameter-group
+ 选项组
  - Name: deeplearnaws-db-option-group

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS