S3 - 区域间复制 - 企业常用, 考试必考之内容
=====================================

## 知识点

* S3 存储桶内容在全球区域间进行复制

## 官网

https://docs.aws.amazon.com/zh_cn/AmazonS3/latest/userguide/replication.html

## 实战演习

+ 在东京区建立存储桶
  - Name: woyaofuzhi
  - 启用版本控制
+ 在新加坡区建立存储桶
  - Name: woyaofuzhibackup
  - 启用版本控制
+ 在东京区建立复制规则
  - 指定全文件
  - 复制到新加坡区存储桶
  - 启用复制时间控制(S3 RTC)
+ 查看复制结果
  - 一般需要等待15分钟左右
  - 错误排查
    * https://docs.aws.amazon.com/zh_cn/AmazonS3/latest/userguide/replication-troubleshoot.html

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
