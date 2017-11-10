---
title: HEXO & GITHUB 搭建个人博客
date: 2017-03-22 16:34:26
tags: 随笔
---
## 配置环境:
#### 1. Git
> 安装 git 客户端 -> [Git官网](https://git-scm.com/downloads)

#### 2. Node.js
> 安装 Node.js -> [Node.js 官网](https://nodejs.org/en/) 或 [中文网](http://nodejs.cn/)  

<!-- more -->
#### 3. Hexo
> 执行完前两步之后,安装 Hexo, 在命令行中输入 `npm install -g hexo-cli`
` // 建立一个博客文件夹, 并初始化博客, <folder> 为文件夹的名称 `  
`$ cd <folder> `  
` $ hexo init `  
` // 生成静态页面 `  
` $ hexo generate or hexo g`  
` // 本地启动`  
` $ hexo server`

#### 4. GitHub
> [官网](https://github.com/) github可以免费托管你的blog，详情参见ggithub help. 也可以自己购买域名+空间

## 基于HEXO GITHUB 搭建个人博客
#### 1. github
注册账号，创建仓库，搞定 <username>.github.io
#### 2. hexo 配置
打开主目录下的 \_config.yml  
写入github配置:  
`deploy: `  
`  type: git `  
`  repository: git@github.com:<username>/<username>.github.io.git `  
`  branch: master `

#### 3. 部署
` // 生成静态页面 `  
` $ hexo generate `  
`  // 部署 `  
`  $ hexo deploy `  
访问 username.github.io
