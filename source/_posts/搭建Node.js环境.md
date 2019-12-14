---
title: 搭建 Node.js 环境
author: IVAn
cover: /images/post_5.jpg
tags:
  - Node.js
  - Window 10
categories: 前端
abbrlink: 27ec92d2
---

Node.js 是一个基于 Chrome V8 引擎的 JavaScript 运行时。 

## Node

### 配置本地 node 环境
  1.<font color=#c7254e>node</font>[官网](https://nodejs.org/en/ "官网")下载。
  ![](http://blog.famuzhe.cn/qianduan/node.js/27ec92d2/node.js1.jpg)

  2.默认安装
  ``` bash
  $ node -v
  $ npm -v
  ```
  ![](http://blog.famuzhe.cn/qianduan/node.js/27ec92d2/node.js2.jpg)

#### 修改
  ``` bash
  $ npm config set registry http://registry.npm.taobao.org/   //修改淘宝源
  ```
#### 还原
  ``` bash
   $ npm config set registry https://registry.npmjs.org/   //还原默认下载源
  ```

#### 查看
  ``` bash
   $ npm config get registry    //查看下载源
  ```
  ![](http://blog.famuzhe.cn/qianduan/node.js/27ec92d2/node.js3.jpg)
