# Jekyll 目录结构

#### Jekyll 核心是一个文本转换引擎。可以通过Markdown、Textile、html等实现目的

- Jekyll 网站的目录结构

<pre>
	_config.yml
	_drafts
		some-drafts.markdown
	_includes
		header.html
		footer.html
		context.html
	_layouts
		default.html
		post.html
		page.html
	_posts
		2015-10-12-how-to-use-markdown.md
		2015-12-10-hello-world.textile
	_data
		socil.yml
	_site
	index.html
	about.md
</pre>

1. _config.yml
	- 保存主要配置数据，同时可通过配置命令行中的设置。如读取指定目录，编码，时区，排除文件等.

2. _drafts
	- drafts 是保存未发布的文章，没有日期。相当于草稿文件
	- drafts 草稿文件当运行`jekyll server` 或 `jekyll build --drafts`  
		将添加自动添加时间生成最新文章。

3. _includes
	- 保存一些包文件用于在布局或文章中加载使用
	- 通过{% include file.ext %} 把文件 `_includes/file.ext`包含进去

4. _layouts
	- 存放文章的模板文件，文章布局可以根据YAML头信息声明进行选择。
	- `{{ content }}` 可将content 插入页面

5. _posts
	- 存放文章的地方，格式必须符合year-month-day-title.markup(markup 可以使md,markdown,textile等)
	
6. _data
	- 存放一些数据，添加额外功能

7. _site
	- 存放Jekyll 转换完成的页面文件

8. index.html
	- 通过包含YAML 头信息，Jekyll自动识别并进行转换。

9. Other
	- 可添加一些其他文件，如css，images 到根文件夹，Jekyll会根据需求自动拷贝。
