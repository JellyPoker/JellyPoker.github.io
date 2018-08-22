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

## 用到的工具或软件
1.[Github Desktop](https://desktop.github.com/)
2.[Jeklly Editor]()

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
**举例说明：(这里以NexT主题项目为例)**
1.在Github上搜索[NexT](https://github.com/simpleyyt/jekyll-theme-next) ，点击Clone or Download中的Download Zip下载压缩包到本地。
2.解压生成文件夹，找到config.yml文件（配置文件），根据自己网站的信息适当修改配置文件。
3.将上述文件夹里的所有内容Push到自己的Github仓库（上面已经创建的名为用户名.github.io的Respository）里，即可应用成功。这一步涉及的文件较多，容易产生冲突，可以用[Github Desktop](https://desktop.github.com/) (Github官方发布的一款笔记本端管理软件)来辅助。
*下面描述具体步骤*


## 撰写博文
## 管理博文
