---
title: 安装 Hexo
categories:
  - blog
tags:
  - hexo
---

[Hexo 官网](https://hexo.io/zh-cn/)

### 准备

**[Git for Windows](https://git-scm.com/download/win)**
**[Node.js](https://nodejs.org/zh-cn/)**

### 安装

```bash
$ npm install hexo-cli -g
$ hexo init blog
$ cd blog
$ npm install
$ hexo server
```

### 命令

#### 创建分类页

```bash
$ hexo new page categoties
```

修改 source/categories/index.md

```bash
---
title: 分类
type: "categories"
---
```

#### 创建标签页

```bash
$ hexo new page tags
```

修改 source/tags/index.md

```bash
---
title: 标签
type: "tags"
---
```

#### 创建关于页

```bash
$ hexo new page about
```

#### 新建一篇文章

```bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/zh-cn/docs/writing)

#### 运行本地服务

```bash
$ hexo clean && hexo s
```

More info: [Server](https://hexo.io/zh-cn/docs/server.html)

#### 部署到远程

```bash
$ hexo clean && hexo d
```

More info: [Deployment](https://hexo.io/zh-cn/docs/deployment.html)
