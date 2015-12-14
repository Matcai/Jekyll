# Jekyll 学习笔记

Jekyll 静态网页生成神器。有了它，妈妈再也不用担心我弄不了博客了啊哈

> 学习参考：http://www.zhanxin.info 和 http://jekyll.bootcss.com

> 感谢上诉网站提供的资料。


### Jekyll 简介

- Jekyll 是一个博客动态生成静态站点的工具。类似WordPress
- Jekyll 不需要数据库的支持，但可以配合第三方服务
- Jekyll 可以免费在Github 上部署。

----

### Jekyll 的安装

1. 首先需要安装ruby 环境
	- Debian 系列通过 apt-get install ruby 
	- Readhat 系列通过 yum install ruby
	- `Ruby 版本不能低于2.0`

2. 安装RubyGems

3. 安装Jekyll
	- gem sources --remove https://rubygems.org/  
		#已被墙，需要更换地址
	- gem sources -a https://ruby.taobao.org/  
		#添加淘宝的源
	- gem sources -l  
		#查看地址
	- gem update --system  
		# 更新软件，可以跳过。
	- gem install jekyll  
		#安装Jekyll

4. 如运行报错 Missing dependency: rdiscount
	- gem install rdiscount  
		#安装rdiscount依赖包。


