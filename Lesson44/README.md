Cloud9 - 建立自己的开发环境
========================

## 知识点

* 建立自己的 Cloud 9 开发环境

## 实战演习

### 建立环境

+ Name: deeplearnaws-cloud9
+ Create a new EC2 instance for environment (direct access)
+ t2.micro (1 GiB RAM + 1 vCPU)
+ Amazon Linux 2 (recommended)
+ Cost-saving setting: After 30 minutes
+ VPC
  - deeplearnaws-vpc
  - deeplearnaws-web-1a

### 环境确认

```bash
# 各种内置软件版本确认
$ aws --version
$ node -v
$ npm -v
$ tsc --version
$ python -V
$ pip -V
$ php -v
$ ruby -v
$ go version
$ java -version
$ g++ -v
$ git version
$ docker version
```

### Node.js

*app.js*

```js
console.log("Helo Cloud9.")
```

```bash
$ node app.js
```

### Python

*main.py*

```python
print("Helo Cloud9.")
```

```bash
python main.py
```

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
