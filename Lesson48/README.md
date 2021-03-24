S3 - 静态网站之王, 快速建立网站之首选
=================================

## 知识点

* 使用 S3 快速搭建静态网页网站
* 使用 Route 53 服务解析网站域名

## 实战演习

+ 设计域名
  - Name: blog.deeplearnaws.ml
+ 建立同名的 S3 存储桶
+ 上传网页文件到存储桶当中
+ 设置存储桶为静态网站公开
+ 设置 Route53, 关联 S3 存储桶
+ 确认动作

*https部分将配合 Cloudfront + AWS Certificate Manager(ACM) 完成, 专门做专题分享*

### index.html

```html
<!DOCTYPE html>
<html lang="zh-cn">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>深学AWS</title>
</head>
<body>
    <h1>你好，AWS。</h1>
</body>
</html>
```

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
