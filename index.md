---
layout: home
title: Asura Blog
---

欢迎来到 Asura Blog！

这是一个简洁清爽的博客平台，专注于分享有价值的内容。

## 最新文章

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%Y年%m月%d日" }}
{% endfor %}

[查看所有文章](/archive.html)
