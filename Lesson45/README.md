Cloud9 - Node.js的开发与调试
===========================

## 知识点

* 在 Cloud9 环境中开发调试 Node.js 应用程序

## 实战演习

```bash
$ mkdir expressweb
$ cd expressweb
$ npm init -y
$ npm install express --save
$ nano app.js
...
$ curl http://httpbin.org/ip
$ node app.js
```

### app.js

```js
'use strict';
const express = require("express")
const app = express()

/////////////////////////////////////////////////
// 定义中间件(进阶)
/////////////////////////////////////////////////
const debug = (req, res, next) => {
    console.log("middleware.debug ->", req.method, req.url)
    next()
}
app.use(debug)

/////////////////////////////////////////////////
// 基础使用
/////////////////////////////////////////////////
// 默认根路径
app.get("/", (req, res) => {
    console.log("->", req.url)
    res.send("<h1>Helo Cloud9.</h1>")
})

// 返回json格式，API主用
app.get("/json", (req, res) => {
    res.json({
        result: 'ok'
    })
})

/////////////////////////////////////////////////
// 启动服务
/////////////////////////////////////////////////
const PORT = process.env.PORT || 8080
app.listen(PORT, (err) => {
    if (err) {
        console.error("我去，出错啦！",)
    }
    console.log("正常服务中...", "http://127.0.0.1:" + PORT)
})
```

## 小马部落(Discord)

https://discord.gg/VSKw72P

## 小马视频频道

http://komavideo.com

## 课程文件

https://github.com/komavideo/LearnAWS
