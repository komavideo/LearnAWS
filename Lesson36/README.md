连接MySQL - MySQL客户端工具
==========================

## 知识点

* 安装 MySQL 客户端工具，连接到 MySQL RDS 数据库实例

## 实战演习

+ 安装 MySQL 客户端命令行工具
+ 连接到 MySQL 服务器实例
+ 建立数据表
+ 添加数据

## Let's Go

```bash
$ sudo yum -y update
$ sudo yum -y install mysql
$ mysql -h mysqldev.cbcbjcjywvwn.ap-northeast-1.rds.amazonaws.com -u root -p
Enter password:
mysql> show databases;
mysql> use blogdb;
mysql> create table blogdb.user (id int, name varchar(255));
mysql> show tables;
mysql> insert into blogdb.user values (1, 'Koma');
mysql> insert into blogdb.user values (2, 'Xiaoma');
mysql> insert into blogdb.user values (3, 'MySql');
mysql> select * from blogdb.user;
mysql> exit;
```

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS