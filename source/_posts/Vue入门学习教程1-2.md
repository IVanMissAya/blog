---
title: Vue入门学习教程1-2
author: IVAn
cover: 'https://ivan-picgo.oss-cn-shenzhen.aliyuncs.com/vue.jpg'
tags:
  - Vue
categories: Vue
abbrlink: 9fa84790
date: 2020-04-02 08:10:00
---
Vue入门学习教程1-2
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190226102947464.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0lWYW5MeWY=,size_16,color_FFFFFF,t_70)
现在我们也来创建一个 .vue的文件
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190226103040847.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0lWYW5MeWY=,size_16,color_FFFFFF,t_70)

然后  
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190226103902196.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0lWYW5MeWY=,size_16,color_FFFFFF,t_70)
这个就是一个组件模板  然后

```
<script>
//导入模板  
export default {
		name: 'firstVue', //这个模板的名称
		props: {
			msg: String    //模板里面参数的类型
		}
	}
</script>
```

```
//这里是写样式的地方
<style>
	#head {
		color: purple;
	}
</style>
```

然后 找到 App.vue
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190226104141689.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0lWYW5MeWY=,size_16,color_FFFFFF,t_70)

```
<script>
	import HelloWorld from './components/HelloWorld.vue'
	import firstVue from './components/first.vue'  //这里就是导入刚刚写的那个模板

	export default {
		name: 'app',
		components: {
			HelloWorld,
			firstVue     //模板名字和first.vue文件里面的模板名称一样
		}
	}
</script>
```

```
<template>
	<div id="app">
		<img alt="Vue logo" src="./assets/logo.png">
		<HelloWorld msg="Welcome to Your Vue.js App" />
		<!--这里就是引用了firstVue这个模板 然后赋值给组件  -->
		<firstVue msg="这是一个组件" />   
	</div>
</template>
```

## 然后这个时候去浏览器看看
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190226104551939.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0lWYW5MeWY=,size_16,color_FFFFFF,t_70)这样我们刚写的哪个组件就导入进去了 、可能看到这里有点不明白！ 然后 我们一起去 public文件夹下面的index.html 去看看
![在这里插入图片描述](https://img-blog.csdnimg.cn/2019022610464965.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0lWYW5MeWY=,size_16,color_FFFFFF,t_70)
这里只有一个 id为app 的div 
然后 我们再去看看 main.js 
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190226104847123.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L0lWYW5MeWY=,size_16,color_FFFFFF,t_70)
这里 import 引入了 App.vue这个组件  然后挂载点就是 index.html里面 id为app的div这个节点。
看到这里是不是 顿时明白了一点什麽
是的 没错！！ 其实App.vue是一个组件  然后 main.js 将App.vue这个组件挂载到了index.html 
然后 那个 HelloWorld.vue 包括刚写的 first.vue 
都做为了  **子组件**  放在App.vue中
懂了吧....



最后最后  如果你还没懂  

**预知后事如何 请看下回分解**
