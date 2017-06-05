---
title: Hexo的同步与更新
date: 2017-06-04 09:30:57
tags: [Hexo]
categories: 其它
---

---

## 同步

### 本地项目

``` bash
$ git pull
```

### 下载项目

``` bash
$ git clone https://github.com/hyphhh/hyphhh.github.io.git
$ git hyphhh.github.io
$ npm install hexo
$ npm install
$ npm install hexo-deployer-git
$ npm install hexo-renderer-less --save
$ npm install hexo-generator-feed --save
$ npm install hexo-generator-json-content --save
```

---

## 更新

### 添加新markdown

``` bash
$ hexo new "My New Post"
```

### 把项目同步到branch *hexo*

``` bash
$ git add .
$ git commit -m "blabla"
$ git push origin hexo
```

### 发布页面到branch *master*

``` bash
$ hexo install hexo-deployer-git --save
$ hexo generate -deploy
```
