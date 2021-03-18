AWS CLI 授权设置(Credential file settings)
=========================================

## 知识点

* AWS CLI 授权设置
  - 建立IAM用户，创建访问密钥
  - 授权CLI身份

## 实战演习

### 建立IAM用户，创建访问密钥

+ Name: deeplearnaws-cli
  - 允许编程访问
  - 建立密钥对(Access Key, Secret Access Key)

### 授权CLI身份

```bash
# 授权CLI身份(指定profile方式 - AWS Best Practices)
$ aws configure --profile deeplearnaws-cli
>AWS Access Key ID [None]: FFUff89898u89vxv
>AWS Secret Access Key [None]: Ahy789yvhjxlFDoajsdflajia90sdfjsaa
>Default region name [None]: ap-northeast-1
>Default output format [None]: json
# 授权文件存储位置(★★★★★内容涉及敏感信息★★★★★)
$ ls ~/.aws
# 列出所有配置数据
$ aws configure list --profile deeplearnaws-cli
# 列出可用配置文件名称
$ aws configure list-profiles --profile deeplearnaws-cli
# 列出当前区的VPC
$ aws ec2 describe-vpcs --profile deeplearnaws-cli
# 查询过滤显示
$ aws ec2 describe-vpcs --profile deeplearnaws-cli --query 'Vpcs[].VpcId'
$ aws ec2 describe-vpcs --profile deeplearnaws-cli --query 'Vpcs[0].VpcId'
$ aws ec2 describe-vpcs --profile deeplearnaws-cli --query 'Vpcs[1].VpcId'
# 列出S3存储桶
$ aws s3 ls --profile deeplearnaws-cli
```

### 删除授权Key

避免安全问题

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
