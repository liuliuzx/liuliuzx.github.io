---
layout: post
title: '免费搭建一个Jekyll站点'
date: 2018-11-27
author: Liuzx.cc
tags: jekyll
---

> 使用Jekyll建立静态博客站点

### 简介

Jekyll

jekyll是一个简单的免费的Blog生成工具，类似WordPress。但是和WordPress又有很大的不同，
原因是jekyll只是一个生成静态网页的工具，不需要数据库支持。
但是可以配合第三方服务,例如Disqus。最关键的是jekyll可以免费部署在Github上，而且可以绑定自己的域名。


### 环境准备

安装 Jekyll 相当简单，但是你得先做好一些准备工作。开始前你需要确保你在系统里已经安装有Ruby。

> 安装Ruby环境  
  
``` bash
$ brew install ruby
$ sudo gem install jekyll
$ sudo gem install jekyll bundler
```
> RubyGems一直以来在国内都非常难访问到，如果Gem安装不上或者很慢怎么办？  

``` bash
$ gem sources --add https://gems.ruby-china.com/ --remove https://rubygems.org/
$ gem sources -l

*** CURRENT SOURCES ***
https://gems.ruby-china.com/
```

> 因为Jekyll项目使用了Gemfile和Bundler，你可以用 Bundler 的 Gem 源代码镜像命令。  

``` bash
$ bundle config mirror.https://rubygems.org https://gems.ruby-china.com
```
  
### 开始

> 新建一个Jekyll项目，注意执行下面的命令会在当前目录新建一个Jekyll项目  

``` bash
$ jkeyll new myblog 
```

> 或者cd到你准备好的目录，Jekyll会在当前目录新建。  
 
``` bash
$ cd /Users/lzx/myblog
$ jkeyll new . 
``` 

### 安装依赖

> 当Jekyll生成博客系统后，可能会有一些依赖，所以还需要在项目目录下安装依赖。  

``` bash
$ sudo bundle install
```

### 启动Jekyll

> 启动Jekyll的命令有几种

``` bash
$ bundle exec jekyll serve
$ jekyll serve
```


### 访问你的Jekyll站点
通过执行Jekyll的命令，可以发行Jekyll已经启动成功了，它的默认地址和端口是[http://127.0.0.1:4000](https://http://127.0.0.1:4000)

Jekyll还有很多地方值得你去发现和了解
* Jekyll 主题
* Jekyll 插件



