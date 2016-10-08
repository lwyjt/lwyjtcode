---
title: first page
date: 2016-09-29 15:01:34
categories: 前言
---

这几天有点闲，索性把学习了下github+hexo搭建部署个人静态博客。踩坑不多，起码去年年底观摩过大神viotgxd
同学的演练之所以现在在自己搭建，原因不外乎本人比较懒了（PS:爆料了自己的一个缺点~）。废话不说，发表下感言。
在这里有几个步骤留下来作为回忆吧！
	1.git的安装
	2.node.js的安装
	3.npm的安装
	  这里注意最新版本的nodeJs已经将npm集成了，安装的时候默认已经安装上了，除非手动选择。
	  此时安装的npm并不是全局的，此时需要将npm设置成全局的，网上baidu了好多，大概也就那样，我是这样做的
		1》Windows下的Nodejs npm路径是appdata，很不爽，想改回来，但是在cmd下执行以下命令
			npm config set cache "D:\nodejs\node_cache"
			npm config set prefix "D:\nodejs\node_global"
		2》在nodejs的安装目录中找到node_modules\npm\.npmrc文件
		修改如下即可：
		prefix = D:\nodejs\node_global
		cache = D:\nodejs\node_cache
		（上面两种可以都试用下，我都改了，不知道只改一项有没有效果，在做的可以使用下）
    4.hexo的安装
	   我这里是新建的目录 D:/hexo
	   右键 git bash
	   执行命令：
	    npm install hexo-cli -g
		hexo init blog
		cd blog
		npm install
		hexo server
		此时在本地浏览器输入localhost:4000/ 出现hexo的页面表示安装成功。
	5.github账号这个就不必说了吧
	6.github的ssh和本机的绑定，这个自行找度娘去吧~
    7.在之前的git bash页面敲入  hexo new hello 
	在blog/sources/_posts创建了hello.md文件
	8.机械化命令：
	  hexo clean
	  hexo generate
	  hexo server
	最后，行动 >>> 心动
