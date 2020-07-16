---
title: Vue入门学习教程1-1
author: IVAn
cover: 'https://static.ivan.fun/blog/vue.jpg'
tags:
  - Vue
categories: -Vue.js
abbrlink: 6a1162a
date: 2020-04-01 08:00:00
---
Vue入门学习教程1-1
# 安装Node.js
node.js官网链接:https://nodejs.org/en/

然后把下载下来的安装包、安装在本地
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190226095425327.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0lWYW5MeWY=,size_16,color_FFFFFF,t_70)

 **检验是否安装成功**
win+R 打开命令行、输入node -v  能看到版本号 则安装成功
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190226095631318.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0lWYW5MeWY=,size_16,color_FFFFFF,t_70)

# 然后下载HBuilderX 这个编译器支持Vue语法、创建Vue项目也很方便
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190226100038146.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0lWYW5MeWY=,size_16,color_FFFFFF,t_70)
安装完之后 新建一个vue项目
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190226100404962.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0lWYW5MeWY=,size_16,color_FFFFFF,t_70)

这个是项目目录结构
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190226100522920.png)
然后选中项目 打开右键菜单 选择外部命令  npm install
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190226100754937.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0lWYW5MeWY=,size_16,color_FFFFFF,t_70)
安装完后的 项目目录结构是这样子的
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190226101521781.png)
这是能看到多出了一个文件夹  node-modules  这个文件夹就是那些依赖包。然后下一步 也是选中项目-外部命令
选择 npm run build  完成之后 项目目录结构是这样子的：
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190226101756832.png)
多了一个dist文件夹  这个文件夹是项目打包后生成的文件夹

最后最后 运行外部命令 npm run server 
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190226102001465.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0lWYW5MeWY=,size_16,color_FFFFFF,t_70)
这样项目就跑起来了  然后浏览器访问 http:localhost:8081

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190226102102540.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0lWYW5MeWY=,size_16,color_FFFFFF,t_70)
一个Vue项目就搭建起来了 嘿嘿~