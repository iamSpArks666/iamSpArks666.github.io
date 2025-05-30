---
layout: default
title: "首页"
---

# 欢迎来到我的博客

这里是我的第一篇首页内容，下面显示最新文章：

<ul>
  {% for post in site.posts limit:5 %}
    <li><a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%Y-%m-%d" }}</li>
  {% endfor %}
</ul>