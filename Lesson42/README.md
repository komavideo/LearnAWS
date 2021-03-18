AWS CLI - 操作EC2实例，一切皆在命令中
=================================

## 知识点

* 使用AWS CLI命令行操作 EC2 实例

## 官网

https://docs.aws.amazon.com/zh_cn/cli/latest/userguide/cli-services-ec2.html

## 实战演习

```bash
# 建立一个EC2实例
$ aws ec2 run-instances --profile deeplearnaws-cli \
    --image-id ami-0ab886fa8b0af1186 \
    --count 1 \
    --instance-type t2.micro \
    --key-name deeplearnaws-ssh-key \
    --subnet-id subnet-0b7f77d791582e6b3 \
    --security-group-ids sg-0e30a29941920eb78 \
    --associate-public-ip-address \
    --tag-specifications 'ResourceType=instance,Tags=[{Key=Name,Value=ec2_from_cli}]'
# 显示EC2内容，赋予过滤条件和查询出哪些字段
$ aws ec2 describe-instances --profile deeplearnaws-cli \
    --filters "Name=instance-type,Values=t2.micro" \
    --query "Reservations[].Instances[].{Instance:InstanceId,Subnet:SubnetId,Instance:Tags}"
# 终止EC2实例
$ aws ec2 terminate-instances --profile deeplearnaws-cli \
    --instance-ids i-03ad4ae25615c672b 
```

## 更多的内容

+ AWS CLI 中文基础开发教学

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
