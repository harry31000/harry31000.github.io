---
layout: default
title: 首頁
---

# 歡迎來到我的專案 Page
這是用 Jekyll theme 的範例。

## 最新文章

{% for post in site.posts %}
  <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
  <p><small>{{ post.date | date: "%Y-%m-%d" }}</small></p>
  <p>{{ post.excerpt }}</p>
{% endfor %}
