# vervel-proxy
最简单的vercel反向代理，两种方式：fork后选择你需要的方式，删除不要的

#### 1. 基于ip（可以加端口）直接代理

{
"version": 2,
"routes": [
{"src": "/(.*)","dest": "http://IP:80/$1"}
]
}

#### 2. 基于域名

{
"version": 2,
"routes": [
{"src": "/(.*)","dest": "https://Your-domain/$1"}
]
}

# 一键部署

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/import/git?s=https://github.com/vtea/vervel-proxy)

