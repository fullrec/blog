---
title: pm2 开机自启动
date: 2019-07-30 13:07:34
categories:
  - 运维
  - pm2
tags:
  - node
  - pm2
---

### 生成启动脚本

```bash
$ pm2 startup
[PM2] You have to run this command as root. Execute the following command:
      sudo su -c "env PATH=$PATH:/home/unitech/.nvm/versions/node/v4.3/bin pm2 startup <distribution> -u <user> --hp <home-path>
```

复制粘贴 sudo su ... 行，执行。_需要 sudo 权限_

### 保存当前进程列表

```bash
$ pm2 save
```

保存进程列表到转储文件 \$PM2_HOME/.pm2/dump.pm2.

### 手动恢复进程

```bash
$ pm2 resurrect
```

恢复以前保存的进程 (pm2 save)

[参考](http://pm2.keymetrics.io/docs/usage/startup/)
