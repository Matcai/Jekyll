## Jekyll YAML 头信息使用方法

----

#### Jekyll YAML的格式必须写在文件的开头，用三个虚线包含在中间。

<pre>
---
layout: post
title: "Hello world"
---
</pre>

- 头信息中可以设置预定义的变量 或者 创建一个 自己定义的变量。
- 这样就可以通过Liquid 标签来访问这些变量


#### 预定义的全局变量

- layout 
	> 指定_layouts 目录下的模板文件

- permalink 
	> 配置访问该文件的指定路径，相当路径映射

- published
	> 设置为 `false` 将展示不具体博文

- category | categories
	> 指定分类属性，使博文能够根据分类属性来阅读
	> 多个类别通过 YAML list 来指定，或者用空格隔开

- tags
	> 类似分类，给文章添加标签
	> 多个标签通过 YAML list 来指定，或者用空格隔开

----

#### 自定义变量

- 自定义变量可通过Liquid 模板调用

- 调用方法：

<pre> 

	<html>
		<head>
			<title>{{ page.title }}</title>
		</head>
	</html>
	...

</pre>

- 通过文章预定义`date`变量
- 会覆盖文件名的日期，达到更新时间分类的效果


