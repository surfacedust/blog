---
title: git 备忘录
date: 2017-12-23 11:17:40
tags:随笔
---
## 配置
安装后需要的配置  
git config --global user.name "John Doe"  
git config --global user.email johndoe@example.com  
如果需要配置编辑器:
git config --global core.editor emacs  
默认是 vim  
查看配置: git config --list  


## 新建项目
已有项目添加到git管理  
1. git init
2. git add .
3. git commit


##从远程版本获取已有项目
1. git clone https://github.com/libgit2/libgit2

## 忽略文件
.gitignore  
### Tip
`GitHub 有一个十分详细的针对数十种项目及语言的 .gitignore 文件列表，你可以在 https://github.com/github/gitignore 找到它.`

## 常用命令
文件
1. 检查工作目录下文件状态：git status || git status -s [简洁的显示文件状态]  
2. git commit -a 如果只是修改了文件，可以直接使用此命令提交
3. git log -p -2 一个常用的选项是 -p，用来显示每次提交的内容差异。 你也可以加上 -2 来仅显示最近两次提交