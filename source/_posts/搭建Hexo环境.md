---
title: 搭建 Hexo 环境
author: IVAn
cover: /images/post_6.jpg
tags:
  - Hexo
  - Window 10
categories: 前端
abbrlink: 9332da2a
---
Hexo 是一个快速、简洁且高效的博客框架。Hexo 使用 Markdown（或其他渲染引擎）解析文章，在几秒内，即可利用靓丽的主题生成静态网页。

## Node.js
  安装[Node.js环境安装](https://www.ivan.fun/2019/12/04/%E6%90%AD%E5%BB%BANode.js%E7%8E%AF%E5%A2%83/ "Node.js环境安装")

## Git
  安装[Git环境安装](https://www.ivan.fun/2019/12/04/%E6%90%AD%E5%BB%BAGit%E7%8E%AF%E5%A2%83/ "Git环境安装")
## Hexo

### 安装Hexo环境
  ``` bash
  $ npm install -g hexo-cli
  $ hexo
  ```
  1.如果显示下面情况，恭喜你成功全局模块调用
  ![](http://blog.famuzhe.cn/qianduan/hexo/9332da2a/hexo1.jpg)

  ``` bash
  $ hexo -v //查看版本
  ```
 ![](http://blog.famuzhe.cn/qianduan/hexo/9332da2a/hexo2.jpg)

  2.随便找个地方初始化文件，执行如下命令：
  ``` bash
  $ mkdir hexo-blog
  ```

  ### 初始化hexo项目
  1.在hexo-blog文件下初始化
  ``` bash
  $ cd hexo-blog
  $ hexo init && npm install
  ```

  2.下载主题
  ``` bash 
  $ git clone https://github.com/iissnan/hexo-theme-next themes/next
  ```
  在本地配置文件中设置theme属性
![](http://blog.famuzhe.cn/qianduan/hexo/9332da2a/hexo3.jpg)

  3.hexo和GitHub关联起来，修改配置文件_config.yml(github中要新建一个仓库用户名+github.io或者搭建[私人Git服务器](http://www.famuzhe.cn/p/c8814d8f/ "私人Git服务器"))
  ``` bash
  deploy:
    type: git
    repo: git@github.com:TeaGardenia/TeaGardenia.github.io.git
    branch: master
  ```
  4.安装deploy-git部署命令
  ``` bash
  npm install hexo-deployer-git --save
  ```


  5.运行hexo项目
  ``` bash
  $ hexo  claen  //清除缓存文件
  $ hexo  generate  //生成静态文件
  $ hexo  server  //启动服务器。默认情况下，访问网址为： http://localhost:4000
  $ hexo  deploy  // 部署网站。
  ```
  打开  http://localhost:4000  验证效果
