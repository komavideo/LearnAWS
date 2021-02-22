建立EC2实例 - 开启我们的云端服务器之旅
=================================

## 知识点

* 建立一个公网可访问的EC2服务器实例

## 实战演习

### EC2实例具体设置

+ Amazon Linux 2 AMI
+ t2.micro
+ deeplearnaws-vpc
+ deeplearnaws-web-1a
+ 自动分配公有 IP
+ 内网IP: 172.16.10.10/32
+ Name: deeplearnaws-web1
+ 密钥对: deeplearnaws-ssh-key

### SSH连接

```bash
$ cp ~/Downloads/deeplearnaws-ssh-key.pem ./
$ chmod 400 deeplearnaws-ssh-key.pem
# Amazon Linux 2
$ ssh -i ./deeplearnaws-ssh-key.pem ec2-user@13.115.167.6
>
```

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
