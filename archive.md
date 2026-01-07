---
layout: page
title: 历史文章
permalink: /archive/
---

<div class="archive-container">
  {% for post in site.posts %}
    {% assign currentDate = post.date | date: "%Y年%m月" %}
    {% assign postDate = post.date | date: "%Y年%m月" %}
    
    {% if currentDate != previousDate %}
      {% unless forloop.first %}</div>{% endunless %}
      <h2 class="archive-month">{{ currentDate }}</h2>
      <div class="archive-posts">
      {% assign previousDate = currentDate %}
    {% endif %}
    
    <div class="archive-post card">
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p class="post-meta">
        <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y年%m月%d日" }}</time>
        {% if post.categories.size > 0 %}
          • 分类：
          {% for category in post.categories %}
            <span class="tag">{{ category }}</span>
          {% endfor %}
        {% endif %}
      </p>
      {% if post.excerpt %}
        <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      {% endif %}
    </div>
    
    {% if forloop.last %}</div>{% endif %}
  {% endfor %}
</div>

<style>
.archive-container {
  margin-top: 2rem;
}

.archive-month {
  color: var(--primary-color);
  border-bottom: 2px solid var(--secondary-color);
  padding-bottom: 0.5rem;
  margin-top: 2rem;
  margin-bottom: 1rem;
}

.archive-posts {
  margin-bottom: 2rem;
}

.archive-post {
  margin-bottom: 1rem;
}

.archive-post h3 {
  margin-bottom: 0.5rem;
}

.archive-post h3 a {
  color: var(--primary-color);
  text-decoration: none;
}

.archive-post h3 a:hover {
  color: var(--secondary-color);
}

.post-excerpt {
  color: #7f8c8d;
  font-size: 0.95rem;
  line-height: 1.5;
  margin-top: 0.5rem;
}
</style>