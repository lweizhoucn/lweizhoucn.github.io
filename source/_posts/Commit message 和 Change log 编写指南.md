---
title: Commit message 和 Change log 编写指南
date: 2020-08-17T10:32:41+08:00
tags:
---
Git 每次提交代码，都要写 Commit message（提交说明），否则就不允许提交。

```shell
git commit -m "hello world"
```

上面代码的-m参数，就是用来指定 commit mesage 的。

如果一行不够，可以只执行git commit，就会跳出文本编辑器，让你写多行。

```shell
git commit
```

目前，社区有多种 Commit message 的写法规范。本文介绍[Angular 规范](https://docs.google.com/document/d/1QrDFcIiPjSLDn3EL15IJygNPiHORgU1_OOAqWjiDU5Y/edit#heading=h.uyo6cb12dt6w)，这是目前使用最广的写法，比较合理和系统化，并且有配套的工具。

## 一、Commit message 的作用

格式化的Commit message，有几个好处。

1. 提供更多的历史信息，方便快速浏览。
比如，下面的命令显示上次发布后的变动，每个commit占据一行。你只看行首，就知道某次 commit 的目的

2. 可以过滤某些commit（比如文档改动），便于快速查找信息。

比如，下面的命令仅仅显示本次发布新增加的功能。

```shell
git log <last release> HEAD --grep feature
```

test
