# Jekyll 快速指南

###  生成静态页面魔板

	jekyll new myblog
	
	cd myblog

	jekyll server

> 通过浏览 http://127.0.0.1:4000 即可查看效果,就这么简单。



### **基本用法**

- jekyll build
	- 生成内容到默认./_site 文件夹中

- jekyll build --destination <destination>
	- 指定生成内容到目标文件夹中

- jekyll build --source <source> --destination <destination>
	- 指定源文件生成内容到目标文件夹中

- jekyll build --watch
	- 生成内容到文件夹并监视内容改变自动生成。

### **服务运行**

- jekyll server
	- 运行服务在 http://localhost:4000/

- jekyll server --detach
	- 后台运行服务监视 http://localhost:4000/

- jekyll server --watch
	- 运行服务并自动查看变更生成页面。

