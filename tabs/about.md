---
title: About

# The About page
# v2.0
# https://github.com/cotes2020/jekyll-theme-chirpy
# © 2017-2019 Cotes Chung
# MIT License
# 此页面显示在站点左侧的about区域
---

## 为什么要搭建个人网站

源于要记录一些个人在语言学习中的内容，方便以后可以快速回忆相关内容

## 为什么选择GitHub Page

想有一个可以存储写的内容的线上站点，这样可以方便自己随时查看，也可以分享一些内容，在网上看了一些平台和内容分享方式，觉的博客是比较合适的，它是个人的，而且方便管理

找了一些已有的博客网站，CSDN、博客园等，觉得页面无法定制，而且看上去也不是很友好，决定搭建一个自己的站点，于是选择了购买云服器，看了一下每年的价格，呃，还是算了，毕竟站点只做记录，每年花个好几百还是舍不得

然后继续找找找，就看到了用GitHub Page搭建个人博客站点，它免费，而且页面可以自己定制，数据库也无需创建，唯一的不足就是要在本地搭建站点环境，这样就只能在本地电脑上做网站的优化和修改了，换个电脑还得重新搭建环境。虽然在本地搭环境这一步不是必须的，可以每次修改了提交到github上看结果，但每改一点就提交到github，这也不太方便，所以还是要搭建本地站点环境的。如果购买了云服务，可以直接在服务器上修改吧（这个也没有试过）。当然了也可以用容器进行环境的迁移等，没弄。

## 什么是GitHub Page

首先，要知道什么是gtihub（Git、GitHub、GitLab待写）

GitHub上存放了项目的源代码，如果一上来就只看代码，结果就是，不做了...，为了每个学习者能看到一个简明易懂的网页，用于说明项目的一些内容，github设计了Pages功能，允许用户自定义项目首页，用来替代默认的源码列表，因此，github Pages可以被认为是用户编写的、托管在github上的静态网页。

## 记录自己在GitHub上搭建站点的过程

可以在网页搜索方法，整个网站的搭建用到的网址如下

查询如何在github上搭建，有很多好的博客，多浏览几个不同的网址，进去做一个大致的了解

之后会发现github page所支持的jekyll，它的英文网站（建议看英文文档，中文文档更新不全面，也不及时）：https://jekyllrb.com/

还会发现可以选择基于jekyll的主题直接使用：http://jekyllthemes.org/，而不用jekyll再去构建网站

选择一个主题开始搭建，之后的搭建步骤，以及符合主题的博客的书写结构等在主题的文件中都有讲解，我使用的主题：http://jekyllthemes.org/themes/jekyll-theme-chirpy/，主题源码地址：https://github.com/cotes2020/jekyll-theme-chirpy/，主题教程地址：https://chirpy.cotes.info/，这两个地址在主题页上都有相应的入口

在github上搭建使用此主题有些建议：

1. 此主题建议使用linux系统搭建，因为它编写的命令适用于linux，我最开始直接用win，没有出现什么问题，因为win10系统有子系统linux，后面在运行tools/run.sh文件中的`bundle exec jekyll s`命令时，因为在win上安装的ruby所在路径不符合linux的文件系统路径，所以提示找不到文件，所以最后改用linux搭建了，另外用win还需要解决搭建过程中运行.sh文件格式的问题，在github上最开始fork的主题没有这个问题，后面fork的就存在此问题
2. 如果要在本地搭建项目环境，会安装ruby，rubygem，安装完rubygem后，建议将gem源修改成国内源：https://gems.ruby-china.com/
3. 如果需要个性化的更改主题的样式，需要了解jekyll的目录结构、[YAML](https://yaml.org/)等，在jekyll网站都有提及

> 你可能会有其他的搭建过程，比如用Jekyll-bootstrap，还有其他主题网站：http://themes.jekyllrc.org/，这些主题的搭建过程不一定相同，依赖的包也不一样，具体要看它们提供的文档
