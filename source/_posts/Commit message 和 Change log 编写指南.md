---
title: Commit message 和 Change log 编写指南
categories:
  - git
abbrlink: 2910968457
date: 2020-08-17 02:32:41
---
> 转载自 [Commit message 和 Change log 编写指南](http://www.ruanyifeng.com/blog/2016/01/commit_message_change_log.html)

Git 每次提交代码，都要写 Commit message（提交说明），否则就不允许提交。

```shell
git commit -m "hello world"
```
上面代码的-m参数，就是用来指定 commit mesage 的。
<!--more-->

如果一行不够，可以只执行git commit，就会跳出文本编辑器，让你写多行。

```shell
git commit
```

![](./Commit%20message%20和%20Change%20log%20编写指南/1.png)

但是，一般来说，commit message 应该清晰明了，说明本次提交的目的。

![](./Commit%20message%20和%20Change%20log%20编写指南/2.png)

目前，社区有多种 Commit message 的写法规范。本文介绍[Angular 规范](https://docs.google.com/document/d/1QrDFcIiPjSLDn3EL15IJygNPiHORgU1_OOAqWjiDU5Y/edit#heading=h.greljkmo14y0)
（见上图），这是目前使用最广的写法，比较合理和系统化，并且有配套的工具。

## 一、Commit message 的作用

格式化的Commit message，有几个好处。

###1. 提供更多的历史信息，方便快速浏览。
比如，下面的命令显示上次发布后的变动，每个commit占据一行。你只看行首，就知道某次 commit 的目的

```shell
git log <last tag> HEAD --pretty=format:%s
```
![](./Commit%20message%20和%20Change%20log%20编写指南/3.png)

### 2. 可以过滤某些commit（比如文档改动），便于快速查找信息。 

比如，下面的命令仅仅显示本次发布新增加的功能。

```shell
git log <last release> HEAD --grep feature
```

### 3. 可以直接从commit生成Change log。

Change Log 是发布新版本时，用来说明与上一个版本差异的文档，详见后文。

![](./Commit%20message%20和%20Change%20log%20编写指南/4.png)

## 二、Commit message 的格式
***
