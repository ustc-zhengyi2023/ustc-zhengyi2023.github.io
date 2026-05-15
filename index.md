---
layout: page
title: 首页
---

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<script>
window.MathJax = {
  tex: {
    inlineMath: [['$', '$']],
    displayMath: [['$$', '$$']]
  }
};
</script>

<style>
.hero {
    text-align: center;
    padding: 60px 30px;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    border-radius: 20px;
    margin-bottom: 40px;
    box-shadow: 0 10px 40px rgba(102, 126, 234, 0.3);
}
.hero h1 {
    font-size: 2.8em;
    color: #fff;
    margin-bottom: 10px;
    font-weight: 700;
    letter-spacing: 2px;
}
.hero .subtitle {
    font-size: 1.2em;
    color: rgba(255, 255, 255, 0.9);
    margin-bottom: 20px;
}
.hero .avatar {
    width: 120px;
    height: 120px;
    border-radius: 50%;
    border: 4px solid rgba(255, 255, 255, 0.8);
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
    margin-bottom: 20px;
    object-fit: cover;
}
.hero .social-links {
    margin-top: 20px;
}
.hero .social-links a {
    display: inline-block;
    margin: 0 10px;
    padding: 8px 20px;
    background: rgba(255, 255, 255, 0.2);
    color: #fff !important;
    text-decoration: none;
    border-radius: 25px;
    font-size: 0.95em;
    transition: all 0.3s ease;
}
.hero .social-links a:hover {
    background: rgba(255, 255, 255, 0.4);
    transform: translateY(-2px);
}

.section {
    background: #fff;
    border-radius: 16px;
    padding: 35px;
    margin-bottom: 30px;
    border: 1px solid rgba(0, 0, 0, 0.08);
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.05);
    transition: box-shadow 0.3s ease;
}
.section:hover {
    box-shadow: 0 8px 30px rgba(0, 0, 0, 0.1);
}
.section h2 {
    font-size: 1.6em;
    color: #4a5568;
    margin-bottom: 20px;
    padding-bottom: 12px;
    border-bottom: 3px solid #667eea;
    display: inline-block;
}

.interest-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 15px;
}
.tag {
    display: inline-block;
    padding: 6px 16px;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: #fff !important;
    border-radius: 20px;
    font-size: 0.9em;
}

.skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
    margin-top: 20px;
}
.skill-card {
    background: linear-gradient(135deg, #f8fafc 0%, #edf2f7 100%);
    padding: 20px;
    border-radius: 12px;
    border-left: 4px solid #667eea;
}
.skill-card h4 {
    color: #4a5568;
    margin-bottom: 10px;
    font-size: 1.1em;
}
.skill-card p {
    color: #718096;
    font-size: 0.9em;
    margin: 0;
}

.post-list {
    list-style: none;
    padding: 0;
    margin: 0;
}
.post-item {
    display: flex;
    align-items: center;
    padding: 15px 0;
    border-bottom: 1px dashed #e2e8f0;
    transition: all 0.3s ease;
}
.post-item:last-child {
    border-bottom: none;
}
.post-item:hover {
    padding-left: 10px;
    background: linear-gradient(90deg, rgba(102, 126, 234, 0.05) 0%, transparent 100%);
}
.post-date {
    font-size: 0.85em;
    color: #8896a6;
    min-width: 100px;
    font-family: "SF Mono", Monaco, monospace;
}
.post-title {
    flex: 1;
    color: #2d3748;
    text-decoration: none;
    font-weight: 500;
    transition: color 0.3s ease;
}
.post-title:hover {
    color: #667eea;
}
.view-all {
    display: inline-block;
    margin-top: 20px;
    padding: 12px 30px;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: #fff !important;
    text-decoration: none;
    border-radius: 25px;
    font-weight: 500;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(102, 126, 234, 0.4);
}
.view-all:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 20px rgba(102, 126, 234, 0.5);
}

.contact-grid {
    display: flex;
    gap: 15px;
    flex-wrap: wrap;
    margin-top: 15px;
}
.contact-item {
    display: flex;
    align-items: center;
    gap: 10px;
    padding: 12px 20px;
    background: #f7fafc;
    border-radius: 10px;
    color: #4a5568;
    text-decoration: none;
    transition: all 0.3s ease;
}
.contact-item:hover {
    background: #edf2f7;
    transform: translateY(-2px);
}

@media (max-width: 768px) {
    .hero h1 { font-size: 2em; }
    .hero { padding: 40px 20px; }
    .section { padding: 25px; }
    .post-item { flex-direction: column; align-items: flex-start; gap: 5px; }
    .post-date { min-width: auto; }
}
</style>

<!-- 头部区域 -->
<div class="hero">
    <img src="/img/head.jpg" alt="Avatar" class="avatar">
    <h1>Welcome</h1>
    <p class="subtitle">算法 · 技术 · 成长</p>
    <div class="social-links">
        <a href="https://github.com/ustc-zhengyi2023">GitHub</a>
        <a href="/about/">About</a>
        <a href="/posts/">Blog</a>
    </div>
</div>

---

<!-- 关于我 -->
<div class="section">
    <h2>About Me</h2>
    <p>你好！我是一名来自<strong>中国科学技术大学</strong>的学生。</p>
    <p>我的研究方向是<strong>计算数学方向</strong>，技术兴趣包括算法、数据结构以及相关领域。</p>
    <p>在这里分享我的学习笔记、技术心得和生活感悟。</p>
    <div class="interest-tags">
        <span class="tag">算法</span>
        <span class="tag">数据结构</span>
        <span class="tag">计算机视觉</span>
        <span class="tag">机器学习</span>
    </div>
</div>

---

<!-- 技术栈 -->
<div class="section">
    <h2>Skills</h2>
    <div class="skills-grid">
        <div class="skill-card">
            <h4>编程语言</h4>
            <p>Python, C++</p>
        </div>
        <div class="skill-card">
            <h4>开发工具</h4>
            <p>Git,VSCode...</p>
        </div>
        <div class="skill-card">
            <h4>技术领域</h4>
            <p>算法设计...</p>
        </div>
        <div class="skill-card">
            <h4>学术技能</h4>
            <p>LaTeX, PyTorch</p>
        </div>
    </div>
</div>

---

<!-- 最新博客 -->
<div class="section">
    <h2>Recent Posts</h2>
    <ul class="post-list">
        {% for post in site.posts limit:5 %}
        <li class="post-item">
            <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
            <a href="{{ post.url }}" class="post-title">{{ post.title }}</a>
        </li>
        {% endfor %}
    </ul>
    <a href="/posts/" class="view-all">View All Posts →</a>
</div>

---

<!-- 联系我 -->
<div class="section">
    <h2>Contact</h2>
    <p>欢迎交流学习！可以通过以下方式联系我：</p>
    <div class="contact-grid">
        <a href="https://github.com/ustc-zhengyi2023" class="contact-item">
            💻 GitHub
        </a>
        <a href="mailto:zhengyi2023@mail.ustc.edu.cn" class="contact-item">
            📧 Email
        </a>
    </div>
</div>
