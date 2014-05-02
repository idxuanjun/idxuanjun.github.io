---
layout: page
title : 首页
tagline: 把工作变成兴趣
---
{% include JB/setup %}

##### 我的博客记录了学习和生活的过程经历，既为了再次查询时的备忘，也想留下了一路走过的痕迹。

正在学习如何在 `Github` 上创建自己的博客，请等待……

## 存档列表

还从来没有用过 `Jekyll`，正在尝试使用，下面是一些未整理完的文档，可以等待全部整理完成后再次访问。

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date: "%Y年%m月%d日" }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

#### 备注

我在CSDN的博客 [CSDN Blog](http://blog.csdn.net/idxuanjun)


