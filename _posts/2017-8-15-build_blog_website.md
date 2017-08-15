---
layout: post
category: github
title: '基于 github+jekyll+markdown 打造个人博客网站'
tagline: by Snail
tags: 
  - github
  - jekyll
  - markdown
  - ruby
  - jacman
  - next
published: true
---

一直想弄一个博客网站，管理自己的知识和技能，同样也可以方便有需要的人。正好手头的项目快完成了，从昨天开始就着手构建我的博客网站，今天网站终于弄好了，把这个经验记下来。

<!--more-->

### 基本步骤
1.if 有 github账号，转第2步，else 注册[github](https://github.com/)账号  
2.创建仓库：登录github账号后，在右上角点击+加号按钮->点击New repository  
![](https://tomhaisen.github.io/blog/assets/images/001.png)  
创建仓库  
![](https://tomhaisen.github.io/blog/assets/images/002.png)  
回到首页，设置你的仓库：点击settings  
![](https://tomhaisen.github.io/blog/assets/images/003.png)  
滚动到页面底部，source选择master branch  
3.git clone 你新建的仓库到本地  
4.网上下载一个[jekyll模板](http://jekyllthemes.org/)，如果你有时间，也可以自己来实现所有的代码。  
5.把下载的jekyll模板代码替换掉git clone到本地的代码  
6.配置你的网站  
7.上面的工作如果都没有问题，接下来你就可以写你的博客了。  
	注意一点就是，博客名是有规范的 年-月-日-title.md,  
	按照markdown语法写博客内容。文章写完后放到_posts目录下，git push到仓库。
	
### 搭建本地jekyll环境
上面是一个粗的流程，如果你需要在博客写完后自己在本地调试，那就需要本地搭建jekyll环境了。  
首先本地下载一个[ruby](https://link.zhihu.com/?target=https%3A//www.ruby-lang.org/en/)安装包，搭建ruby环境。  
之后就是要安装[RubyGems](https://link.zhihu.com/?target=https%3A//rubygems.org/pages/download),rubygems就是一个包管理器，类似于node.js的npm。

```sh
//在RubyGems官网上下载压缩包，解压到你的本地任意位置
//在Terminal中
cd yourpath to RubyGems //你解压的位置
ruby setup.rb
```
接下来可以安装你的jekyll了

```sh
 gem install jekyll
```


