---
layout: post
title:  "Deep Learning 激活函数总结"
date:   2020-04-18 09:30:54
categories: DL基础
tags: DL
---

* content
{:toc}

虽然搭建博客比较久了，但是没有怎么写笔记；我发现连sigmoid这样的函数都忘了，所以想写个总结。

##  Lost Function 和 Cost Function

在 Andrew Ng 的深度学习课程中，偶然知道:

* Lost Function(损失函数) 指的是在一个样本上衡量预测值和实际值之间的差距；

* Cost Function(成本函数) 衡量（模型）在全体训练样本上的表现

## Sigmoid

函数表达式：$$\sigma(z)=\large \frac{1}{1+e^{-z}}$$

函数图像：![img](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1587274282433&di=3f4c43b2b7d2225f31824178340f48ce&imgtype=0&src=http%3A%2F%2F5b0988e595225.cdn.sohucs.com%2Fimages%2F20181019%2Fa4fe1ff6079142908d7ec4b97fbfb01c.jpeg)





