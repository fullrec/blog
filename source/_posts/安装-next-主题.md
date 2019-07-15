---
title: 安装 Next 主题
date: 2019-07-14 21:11:51
tags: hexo
---

[Next](https://github.com/theme-next/hexo-theme-next) [使用文档](https://theme-next.iissnan.com/)

### 使用 Git 子模块 安装

``` bash
$ git submodule add https://github.com/theme-next/hexo-theme-next themes/next
```

### 修改网站配置

``` yaml
language: zh-CN
timezone: Asia/Shanghai

# ...

theme: next

theme_config: # 启用此选项，不用修改 themms/next/_config.yml 文件。
  menu: 
    home: / || home
    archives: /archives/ || archive
    #about: /about/ || user
    categories: /categories/ || th
    tags: /tags/ || tags
    
  scheme: Gemini
  avatar: 
    url: /images/avatar.jpg
  codeblock:
    highlight_theme: 'night bright' #'night eighties'

```