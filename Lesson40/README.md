AWS CLI 的安装(Install)
======================

## 知识点

* AWS CLI 的安装

## 官网

### AWS CLI v1

https://docs.aws.amazon.com/zh_cn/cli/latest/userguide/install-cliv1.html

### AWS CLI v2

https://docs.aws.amazon.com/zh_cn/cli/latest/userguide/install-cliv2.html

## 实战演习

### 安装Mac CLI v2版本

https://docs.aws.amazon.com/zh_cn/cli/latest/userguide/install-cliv2-mac.html

```bash
#################################################
# 安装版本确认
$ aws --version
```

### 安装Linux(Ubuntu) CLI v2版本

https://docs.aws.amazon.com/zh_cn/cli/latest/userguide/install-cliv2-linux.html

```bash
# 下载最新CLI程序版本
$ curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
# 解压缩
$ sudo apt install -y unzip
$ unzip awscliv2.zip
# 管理员权限安装
$ sudo ./aws/install
# 安装版本确认
$ aws --version
# 使用帮助
$ aws help
```

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
