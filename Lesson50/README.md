S3 - 网关终端节点 - 私有网络访问S3的捷径
===================================

## 知识点

* 通过设置网关终端节点，使私有网段中的EC2也可以访问到S3服务

## 官网

https://docs.aws.amazon.com/zh_cn/codeartifact/latest/ug/create-s3-gateway-endpoint.html

## 实战演习

>看图说话

## 实战步骤

+ 创建一个可以访问S3的角色
  - KomaRoleS3FullAccess
+ 在私有网段启动一个EC2实例, 赋予S3访问的角色
+ 在私有网段EC2中访问S3
+ 在VPC中建立一个网关终端节点，绑定到私有网段的路由表
+ 稍候片刻(添加到路由表需要时间)
+ 再次从私有网段中的EC2访问S3，确认动作

## 动作确认脚本

```bash
$ aws s3 ls --region ap-northeast-1
```

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 深学AWS

https://deeplearnaws.com/

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
