---
layout: home
title: 首页
---

# 欢迎来到我的博客

这是一个分享 Kiro 学习历程和技术心得的个人博客。

## 最新文章

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%Y年%m月%d日" }}
{% endfor %}

## 关于我

我是一名开发者，正在学习和探索 Kiro 这个强大的 AI 编程助手。通过这个博客，我想分享我的学习心得和实践经验。
