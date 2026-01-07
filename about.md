---
layout: page
title: 关于我
permalink: /about/
---

<div class="about-container">
  <div class="about-header">
    <div class="avatar">
      <span class="avatar-emoji">👨‍💻</span>
    </div>
    <h1>你好，我是 hpuhsp</h1>
    <p class="intro">一名热爱技术的开发者，正在探索 AI 辅助编程的奇妙世界</p>
  </div>

  <div class="about-content">
    <div class="section card">
      <h2>🎯 我的兴趣</h2>
      <div class="interests-grid">
        <div class="interest-item">
          <span class="interest-icon">💻</span>
          <span>软件开发</span>
        </div>
        <div class="interest-item">
          <span class="interest-icon">🤖</span>
          <span>AI 编程助手</span>
        </div>
        <div class="interest-item">
          <span class="interest-icon">📝</span>
          <span>技术分享</span>
        </div>
        <div class="interest-item">
          <span class="interest-icon">🚀</span>
          <span>新技术探索</span>
        </div>
      </div>
    </div>

    <div class="section card">
      <h2>📖 关于这个博客</h2>
      <p>这个博客是我学习 Kiro AI 编程助手的记录空间。在这里，我会分享：</p>
      <div class="blog-features">
        <div class="feature-item">
          <span class="feature-icon">🛠️</span>
          <div>
            <h3>Kiro 使用技巧</h3>
            <p>实用的操作方法和高效工作流程</p>
          </div>
        </div>
        <div class="feature-item">
          <span class="feature-icon">⭐</span>
          <div>
            <h3>编程最佳实践</h3>
            <p>代码质量提升和开发规范</p>
          </div>
        </div>
        <div class="feature-item">
          <span class="feature-icon">🎯</span>
          <div>
            <h3>项目开发经验</h3>
            <p>真实项目中的应用案例分享</p>
          </div>
        </div>
        <div class="feature-item">
          <span class="feature-icon">🔧</span>
          <div>
            <h3>问题解决方案</h3>
            <p>常见问题的排查和解决思路</p>
          </div>
        </div>
      </div>
    </div>

    <div class="section card">
      <h2>🌟 我的目标</h2>
      <p>通过这个博客，我希望能够：</p>
      <ul class="goals-list">
        <li>记录自己的学习成长轨迹</li>
        <li>帮助其他开发者更好地使用 Kiro</li>
        <li>建立技术交流和分享的平台</li>
        <li>推广 AI 辅助编程的理念和实践</li>
      </ul>
    </div>

    <div class="section card contact-section">
      <h2>📬 联系我</h2>
      <p>如果你有任何问题、建议或想要交流，欢迎通过以下方式联系我：</p>
      <div class="contact-links">
        <a href="https://github.com/hpuhsp" class="contact-link" target="_blank">
          <span class="contact-icon">🐙</span>
          <span>GitHub</span>
        </a>
        <a href="mailto:your-email@example.com" class="contact-link">
          <span class="contact-icon">📧</span>
          <span>Email</span>
        </a>
      </div>
    </div>
  </div>
</div>

<style>
.about-container {
  max-width: 800px;
  margin: 0 auto;
}

.about-header {
  text-align: center;
  padding: 2rem 0;
  margin-bottom: 2rem;
}

.avatar {
  width: 120px;
  height: 120px;
  border-radius: 50%;
  background: linear-gradient(135deg, var(--secondary-color), #2980b9);
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0 auto 1.5rem;
  box-shadow: 0 8px 25px rgba(52, 152, 219, 0.3);
}

.avatar-emoji {
  font-size: 3rem;
}

.about-header h1 {
  color: var(--primary-color);
  margin-bottom: 0.5rem;
  font-size: 2.2rem;
}

.intro {
  font-size: 1.2rem;
  color: #7f8c8d;
  margin-bottom: 0;
}

.section {
  margin-bottom: 2rem;
}

.section h2 {
  color: var(--primary-color);
  margin-bottom: 1.5rem;
  font-size: 1.5rem;
}

.interests-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 1rem;
  margin-top: 1rem;
}

.interest-item {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.8rem;
  background: var(--code-bg);
  border-radius: 8px;
  border: 1px solid var(--border-color);
}

.interest-icon {
  font-size: 1.2rem;
}

.blog-features {
  margin-top: 1.5rem;
}

.feature-item {
  display: flex;
  align-items: flex-start;
  gap: 1rem;
  margin-bottom: 1.5rem;
}

.feature-icon {
  font-size: 1.5rem;
  margin-top: 0.2rem;
}

.feature-item h3 {
  color: var(--primary-color);
  margin-bottom: 0.3rem;
  font-size: 1.1rem;
}

.feature-item p {
  color: #7f8c8d;
  margin: 0;
  font-size: 0.95rem;
}

.goals-list {
  margin-top: 1rem;
}

.goals-list li {
  margin-bottom: 0.5rem;
  color: var(--text-color);
}

.contact-section {
  text-align: center;
}

.contact-links {
  display: flex;
  justify-content: center;
  gap: 2rem;
  margin-top: 1.5rem;
}

.contact-link {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.8rem 1.5rem;
  background: var(--secondary-color);
  color: white;
  text-decoration: none;
  border-radius: 25px;
  transition: all 0.3s ease;
}

.contact-link:hover {
  background: var(--accent-color);
  transform: translateY(-2px);
  box-shadow: 0 5px 15px rgba(231, 76, 60, 0.3);
  color: white;
  text-decoration: none;
}

.contact-icon {
  font-size: 1.2rem;
}

@media screen and (max-width: 768px) {
  .about-header h1 {
    font-size: 1.8rem;
  }
  
  .intro {
    font-size: 1rem;
  }
  
  .interests-grid {
    grid-template-columns: 1fr;
  }
  
  .contact-links {
    flex-direction: column;
    align-items: center;
  }
}
</style>
