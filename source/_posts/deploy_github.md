---
title: 部署到 github
date: 2019-07-14 04:23:27
tags:
---

### 安装 hexo-deployer-git
``` bash
npm i hexo-deployer-git
```

### 修改配置
```
deploy:
  type: git
  repo: <repository url> #git@github.com:fullrec/fullrec.github.io.git
  branch: [branch] #master
  message: [message] #自定义提交信息 (默认为 Site updated: {{ now('YYYY-MM-DD HH:mm:ss') }})
```

### 生成站点文件并推送至远程库
``` bash
hexo clean
hexo d
```