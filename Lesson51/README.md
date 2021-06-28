Budgets - 使用预算跟踪成本
========================

## 知识点

* 使用预算跟踪成本, 超出预算时发送警告邮件

## 实战演习

### 账单和成本管理控制面板

+ Budgets
  - 预算类型: 成本预算
  - 设置预算金额: $10
  - 预算名称: 我的预算我做主
  - 提醒阈值: 50% 实际预算金额
  - SNS 提醒

### SNS授权

*Deeplearnaws_SNS_Topic*

```json
{
  "Sid": "AWSBudgets-notification-publish",
  "Effect": "Allow",
  "Principal": {
    "Service": "budgets.amazonaws.com"
  },
  "Action": "SNS:Publish",
  "Resource": "arn:aws:sns:ap-northeast-1:976591345876:Deeplearnaws_SNS_Topic"
}
```

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 深学AWS

https://deeplearnaws.com/

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
