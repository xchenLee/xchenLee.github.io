---
layout: post
title:  "使用 github pages 和  Jekyll 建站"
date:   2016-04-20 16:56:51 +0800
categories: jekyll github
---

今天在网上浏览技术帖子，无意看到关于Github建站.就动手做了一下，现在通过查资料搭起来了，先写一篇`post`

关键词搜了很多文章，指引性并不强。其实很多技术上的东西就是动手去做，这些文章跳跃性的纪录其实对初学者并不友好。最后还是找到了 `Github` [官方教程] 写的很清晰

跟着页面的 `User or organization site` 走完五个步骤就建好并浏览自己建的网站了

接下来就是安装和使用`jekyll`了

1.安装前需要电脑装有python，gem

2.然后开始安装gem功能包

{% highlight ruby %}
gem install jekyll   //jekyll
gem install kramdown //markdown 解析包
gem install pygments.rb //代码高亮
gem install liquid
{% endhighlight %}

3.安装完成之后，进入之前五个步骤中拉取repository的文件夹，执行命令

{% highlight ruby %}
jekyll new . --force //直接覆盖五个步骤中新建的index.html
//如果是想新建一个空的
jekyll new name
//然后编辑
jekyll buid
//运行
jekyll serve //打开 localhost:4000就可以看到了

//这个时候就可以提交了
git add .
git commit -m "commit msg"
git push -u origin master
//然后打开你Github域名网站就可以访问了
{% endhighlight %}


[官方教程]: https://pages.github.com
