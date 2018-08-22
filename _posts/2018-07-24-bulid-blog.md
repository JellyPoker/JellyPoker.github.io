---
category: 技术养成
layout: post
tags:
  - GithubPages
  - Jekyll
  - 博客
  - 美化
title: 如何快速搭建个人博客
---
## 前言
  最近正在接触大数据项目的开发，需要学习很多新知识，由于内容繁多且复杂，于是想把自己的学习过程以博客的方式记录下来。因此第一步就是得有一个博客，本文将详细介绍如何用GithubPages以及Jekyll快速搭建个人博客，以及后续如何上传管理博客文章。


## 创建博客站点
### 利用GithubPages自动生成博客站点
&nbsp; &nbsp; &nbsp; &nbsp; GithubPages是一种静态站点生成服务，它可以根据Github中特定的Repository生成静态站点。在其规则下，Github用户只要创建一个Repository并将其命名为特定格式（username.github.io），就能生成一个静态站点可供访问。下面将描述如何建站：
1. 注册Github账号并登录。
2. 创建一个Repository，命名为 用户名.github.io。
3. 点击Settings可查看站点是否已经被成功发布。具体操作：点击Settings下拉页面找到GithubPages查看站点的发布信息，若发布成功，则会显示以下信息：
![网站发布成功](/assets/images/shotpics/p1.jpg)

根据上图，站点已被发布在https://jellypoker.github.io 上，此时可以在浏览器输入该地址即可访问自己所建的站点。
若发布失败有可能是config配置文件编写出错，这里也会显示具体错误出现的行数，便于修改。


### 美化博客站点
经过以上步骤，建站的第一步已经完成，任何人可以通过输入网址访问你的网站。但此时的网站比较简陋，缺少美化，也降低了可用性。因此，下一步我们需要对网站进行美化。推荐的方法是在Github上fork并下载优秀的开源项目，通过修改配置文件将其应用到自己的网站中。
####举例说明：(这里以NexT主题项目为例)
- 1.在Github上搜索[NexT](https://github.com/simpleyyt/jekyll-theme-next) ，点击-Clone or Download中的Download Zip下载压缩包到本地。
- 2.解压生成文件夹，找到config.yml文件（配置文件），根据自己网站的信息适当修改配置文件。
- 3.将上述文件夹里的所有内容Push到自己的Github仓库（上面已经创建的名为用户名.github.io的Repository）里，即可应用成功。这一步涉及的文件较多，容易产生冲突，可以用[Github Desktop](https://desktop.github.com/) (Github官方发布的一款笔记本端管理软件，可事先对其使用说明进行了解)来辅助。
*下面对第3步做详细描述*
- （1）打开Github Desktop，登录自己的Github账号
- （2）点击最上方工具栏File下的Clone Repository，可看到该账号下的Repository，选择名为JellyPoker.github.io的Repository点击Clone将其下载到本地路径(如下图所示)，请记住该路径。
![下载到本地](/assets/images/shotpics/p2.jpg)

- （3）将第2步解压并修改配置文件的文件夹中的所有内容复制粘贴至本地文件夹中（第2步中文件保存的本地路径）。
- （4）此时点开Github Desktop将发现所有的文件修改替换信息全部显示在左侧(如下图)，但这只是本地文件进行了修改替换，Github上的项目文件仍然不变，网站内容和页面也因此不变。所以接下来，我们需要将所有已经修改替换后的文件Push到Github仓库中。在左侧简要填写summary然后点击下面的Commit to master提交修改（如下图），最后点击上方的Push origin将修改push到Github上的仓库（如下图）。
![显示变化并提交修改](/assets/images/shotpics/p3.jpg)
![push到Github上](/assets/images/shotpics/p4.jpg)
- 4.刷新自己的网站，即可发现主题已经运用，美化基本完成。
## 撰写并发布博文
以该方式建立的站点，博文其实是一个md文件（如：ReadMe.md），文件中多采用Markdown语法，[点击了解一下简易Markdown语法](https://jellypoker.github.io/小芝士/2018/08/21/the-post-6392)
写好博文后，将其放在Repository的_posts目录下，即可在网站上发布该博文。方法可以同样是在本地编辑好博文并放入本地文件夹，再通过Github Desktop同步到Github仓库中。
![博文所在位置](/assets/images/shotpics/p5.jpg)
## 管理博文
博文众多，如何管理博文是一个关键点，因为博文多半情况不是一成不变的，后续多需要频繁修改其内容。管理博文可以借助工具，常用的工具有：Jekyll Editor(是一个chrome插件)、[Jekyll Writer](http://jekyllwriter.com/)(是一个桌面应用)。还有其他的管理应用和工具，[可参考这篇文章](http://hechonghua.com/easy-post-jekyll/amp/)
## 结束语
有了上面的教程，快点建站嗨起来吧！