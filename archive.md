---
layout: page
title: 文章归档
permalink: /archive/
---

# 文章归档

## 按年份分类

{% assign posts_by_year = site.posts | group_by_exp: "post", "post.date | date: '%Y'" %}

{% for year in posts_by_year %}
  <h3>{{ year.name }}</h3>
  <ul>
  {% for post in year.items %}
    <li>
      <span class="post-meta">{{ post.date | date: "%m月%d日" }}</span>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
  </ul>
{% endfor %}

---

共 {{ site.posts.size }} 篇文章
