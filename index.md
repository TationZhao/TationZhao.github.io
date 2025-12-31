---
layout: default
title: 首页
---

# Tation 的博客

欢迎来到我的个人站！以下是我最近发布的文章：

---

### 文章列表

{% for post in site.posts %}
* **{{ post.date | date: "%Y-%m-%d" }}** —— [{{ post.title }}]({{ post.url }})
{% endfor %}

{% if site.posts.size == 0 %}
*(目前还没有文章，请检查 _posts 文件夹)*
{% endif %}
