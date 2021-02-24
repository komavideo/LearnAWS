建立私有网段的服务器 - For MySQL
=============================

## 知识点

* 修改私有网段安全组，增加 Port:22 支持
* 在私有网段建立 EC2 实例
* 通过公有网段 web-ec2 实例连接到 db-ec2 实例

## 实战演习

### * 修改私有网段安全组，增加 Port:22 支持

+ deeplearnaws-db-sg
+ Port: 22

### 在私有网段建立 EC2 实例

+ Name: deeplearnaws-db1

### 通过公有网段 web-ec2 实例连接到 db-ec2 实例

+ 本地连接到 deeplearnaws-web1
+ 拷贝本地连接私钥到 deeplearnaws-web1
+ 通过 deeplearnaws-web1 连接到 deeplearnaws-db1
+ deeplearnaws-db1测试

```bash
# @deeplearnaws-web1
$ ssh -i ./deeplearnaws-ssh-key.pem 172.16.20.10
# @deeplearnaws-db1
$ sudo yum update -y
$ curl https://komavideo.com
```

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
