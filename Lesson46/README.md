S3 - AWS的存储核心
=================

## 知识点

* S3的基础知识

## 官网

https://aws.amazon.com/cn/s3

## 基础介绍

Amazon Simple Storage Service (Amazon S3) 是一种对象存储服务，
提供行业领先的可扩展性、数据可用性、安全性和性能。这意味着各种规模和行业
的客户都可以使用 S3 来存储并保护各种用例（如数据湖、网站、移动应用程序、
备份和还原、存档、企业应用程序、IoT 设备和大数据分析）的数据，容量不限。
Amazon S3 提供了易于使用的管理功能，因此您可以组织数据并配置精细调整过
的使用权限控制，从而满足特定的业务、组织和合规性要求。Amazon S3 可达到
99.999999999%（11 个 9）的持久性，并为全球各地的公司存储数百万个应用
程序的数据。

## 用途

+ 数据文件保存
+ 日志文件保存
+ 备份快照保存
+ 静态网站主机
+ 数据湖(data lake)

## 价格

https://aws.amazon.com/cn/s3/pricing

### AWS 免费套餐

作为 AWS 免费套餐的一部分，您可以免费开始使用 Amazon S3。注册后，
AWS 新客户将在一年内的每个月中获得 S3 标准存储类中的 5GB S3 存储空间、
20000 个 GET 请求、2000 个 PUT、COPY、POST 或 LIST 请求以及 15GB
的数据传出量。

## 安全性(重要)

+ SSE-S3
+ SSE-KMS
+ SSE-C
+ CSE

## 存储分类（认证必考内容）

+ S3 标准
  - 适用于频繁访问的数据的通用存储
+ S3 智能分层
  - 适用于具有未知或变化的访问模式的数据
+ S3 标准 - IA
  - 不频繁访问
+ S3 单区 - IA
  - 不频繁访问
+ S3 Glacier
  - 长期存档
+ S3 Glacier Deep Archive
  - 长期存档
+ S3 Outposts
  - 本地存储

*具体区别*

https://aws.amazon.com/cn/s3/storage-classes

## 使用例

### 小马视频

https://komavideo.com

## 今后部署预定

### 深学AWS

https://deeplearnaws.com

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
