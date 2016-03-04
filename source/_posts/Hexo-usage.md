---
title: Hexo usage tips
date: 1000-01-01 00:00:00
tags: hexo
categories: Hexo Usage
description: How to use Hexo
feature:
toc: true
---

# Commands

## init
```
$ hexo init [folder]
```

## new post/page/...
```
$ hexo new [layout] <title>
```
Creates a new article. If no layout is provided, Hexo will use the default_layout from _config.yml. If the title contains spaces, surround it with quotation marks.
也可以在source/_posts/下直接新建*.md文件

## generate
```
$ hexo generate
```
生成静态网页文件
<!--more-->

## 本地查看效果
```
$ hexo server
```
Starts a local server. By default, this is at http://localhost:4000/.

## deploy
```
$ hexo deploy
```
在_config.yml中设置deploy方法。my config:
{% blockquote %}
deploy:
  type: git
  repo: username@xxx.xxx.xxx:hexo_blog.git
{% endblockquote %}
将通过git发布到我的VPS。
有关VPS上的git repo的设置（特别是hooker），参见其他笔记。
有关VPS的登录验证，参见其他笔记。

## github维护代码
和deploy是分开的操作。具体设置参见其他笔记。



