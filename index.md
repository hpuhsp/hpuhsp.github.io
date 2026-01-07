---
layout: home
title: 首页
---

<div class="hero-section">
  <h1 class="hero-title">🚀 欢迎来到 Kiro 学习之旅</h1>
  <p class="hero-description">
    这里记录我与 Kiro AI 编程助手的学习历程，分享实用技巧和开发心得。
    让我们一起探索 AI 辅助编程的无限可能！
  </p>
  <a href="/about/" class="btn hero-btn">了解更多</a>
</div>

<div class="features-section">
  <div class="feature-grid">
    <div class="feature-card card">
      <h3>🎯 学习记录</h3>
      <p>详细记录 Kiro 的使用技巧和最佳实践</p>
    </div>
    <div class="feature-card card">
      <h3>💡 实战经验</h3>
      <p>分享真实项目中的应用案例和解决方案</p>
    </div>
    <div class="feature-card card">
      <h3>🔧 工具技巧</h3>
      <p>探索 Kiro 的高级功能和使用窍门</p>
    </div>
  </div>
</div>

<div class="recent-posts-section">
  <h2>📝 最新文章</h2>
  <div class="posts-grid">
    {% for post in site.posts limit:6 %}
      <article class="post-card card">
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p class="post-meta">
          <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y年%m月%d日" }}</time>
          {% if post.categories.size > 0 %}
            {% for category in post.categories %}
              <span class="tag">{{ category }}</span>
            {% endfor %}
          {% endif %}
        </p>
        {% if post.excerpt %}
          <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 20 }}</p>
        {% endif %}
        <a href="{{ post.url | relative_url }}" class="read-more">阅读全文 →</a>
      </article>
    {% endfor %}
  </div>
  
  {% if site.posts.size > 6 %}
    <div class="view-all">
      <a href="/archive/" class="btn">查看所有文章</a>
    </div>
  {% endif %}
</div>

<style>
.hero-section {
  text-align: center;
  padding: 3rem 0;
  background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
  border-radius: 15px;
  margin-bottom: 3rem;
}

.hero-title {
  font-size: 2.5rem;
  color: var(--primary-color);
  margin-bottom: 1rem;
  font-weight: 700;
}

.hero-description {
  font-size: 1.2rem;
  color: #7f8c8d;
  margin-bottom: 2rem;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
  line-height: 1.6;
}

.hero-btn {
  font-size: 1.1rem;
  padding: 12px 30px;
}

.features-section {
  margin-bottom: 3rem;
}

.feature-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  margin-top: 2rem;
}

.feature-card {
  text-align: center;
  padding: 2rem 1.5rem;
}

.feature-card h3 {
  color: var(--primary-color);
  margin-bottom: 1rem;
  font-size: 1.3rem;
}

.recent-posts-section h2 {
  color: var(--primary-color);
  text-align: center;
  margin-bottom: 2rem;
  font-size: 2rem;
}

.posts-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1.5rem;
  margin-bottom: 2rem;
}

.post-card {
  padding: 1.5rem;
}

.post-card h3 {
  margin-bottom: 0.8rem;
}

.post-card h3 a {
  color: var(--primary-color);
  text-decoration: none;
  font-size: 1.2rem;
}

.post-card h3 a:hover {
  color: var(--secondary-color);
}

.post-excerpt {
  color: #7f8c8d;
  font-size: 0.95rem;
  line-height: 1.5;
  margin: 1rem 0;
}

.read-more {
  color: var(--secondary-color);
  font-weight: 500;
  text-decoration: none;
  font-size: 0.9rem;
}

.read-more:hover {
  color: var(--accent-color);
}

.view-all {
  text-align: center;
  margin-top: 2rem;
}

@media screen and (max-width: 768px) {
  .hero-title {
    font-size: 2rem;
  }
  
  .hero-description {
    font-size: 1rem;
  }
  
  .feature-grid {
    grid-template-columns: 1fr;
  }
  
  .posts-grid {
    grid-template-columns: 1fr;
  }
}
</style>
