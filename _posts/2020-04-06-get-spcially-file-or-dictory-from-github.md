---
layout: post
title:  "从GitHub下载指定文件或者文件夹"
categories: GitHub
tags:  GitHub 工具
author: hughzeng
---

---



电脑已经装好git，有GitHub账号

（1）创建想要存放的文件夹(假设此处想要把下载的文件放在 E:\blog下)，并 `cd`到此文件夹，然后初始化此文件夹：

` git init`

(2)连接GitHub上的远程仓库：

`git remote add -f origin <url>`                                   `<url>`是GitHub得到的下载文件以.git结尾的地址

**（3）开启sparse checkout 模式**

`git config core.sparsecheckout true`

**(4)告诉Git哪些文件或者文件夹是你真正想Check Out的**
 (你可以将它们作为一个列表保存在 .git/info/sparse-checkout 文件中。)

例如：
 `$ echo libs >> .git/info/sparse-checkout`  
 `$ echo apps/register.go >> .git/info/sparse-checkout `   
 `$ echo resource/css >> .git/info/sparse-checkout`  

(5)拉取想要的分支

`git pull origin master`

[这篇博客](https://www.jianshu.com/p/74a0441ed9b7)写得特别详细