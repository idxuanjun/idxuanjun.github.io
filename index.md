---
layout: page
title : 首页
tagline: 把工作变成兴趣
---
{% include JB/setup %}

正在学习如何在 `Github` 上创建自己的博客，请等待……

## 学习中……

还从来没有用过 `Jekyll`,正在学习使用，下面是一些测试的例子，等待转换完成后再次访问。

这里是我的“文章列表”

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date: "%Y年%m月%d日" }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

### 备注

可以先访问我在CSDN的博客 [CSDN Blog](http://blog.csdn.net/idxuanjun)


