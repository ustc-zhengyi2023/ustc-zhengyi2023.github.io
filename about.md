---
layout: page
title: About
permalink: /about/
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
.page-content {
    max-width: 800px;
    margin: 0 auto;
    padding: 40px 20px;
}
.section {
    background: #fff;
    border-radius: 16px;
    padding: 35px;
    margin-bottom: 30px;
    border: 1px solid rgba(0, 0, 0, 0.08);
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.05);
}
.section h2 {
    font-size: 1.5em;
    color: #4a5568;
    margin-bottom: 20px;
    padding-bottom: 12px;
    border-bottom: 3px solid #667eea;
    display: inline-block;
}
.section h3 {
    font-size: 1.2em;
    color: #2d3748;
    margin: 20px 0 10px 0;
}
.section p {
    color: #555;
    line-height: 1.8;
    margin-bottom: 12px;
}
.section ul {
    list-style: none;
    padding: 0;
}
.section li {
    padding: 8px 0;
    color: #555;
    padding-left: 25px;
    position: relative;
}
.section li::before {
    content: "▸";
    color: #667eea;
    position: absolute;
    left: 0;
}
.skill-tag {
    display: inline-block;
    padding: 4px 12px;
    background: linear-gradient(135deg, #f8fafc 0%, #edf2f7 100%);
    border-radius: 15px;
    margin: 4px;
    font-size: 0.9em;
    color: #4a5568;
    border: 1px solid #e2e8f0;
}
.contact-row {
    display: flex;
    gap: 15px;
    flex-wrap: wrap;
    margin-top: 15px;
}
.contact-btn {
    display: flex;
    align-items: center;
    gap: 8px;
    padding: 12px 20px;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: #fff !important;
    text-decoration: none;
    border-radius: 10px;
    font-weight: 500;
    transition: all 0.3s ease;
}
.contact-btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 15px rgba(102, 126, 234, 0.4);
}
.back-link {
    display: inline-block;
    margin-bottom: 20px;
    color: #667eea;
    text-decoration: none;
    font-weight: 500;
}
.back-link:hover {
    text-decoration: underline;
}
</style>

<a href="/" class="back-link">← Back to Home</a>

<div class="section">
    <h2>About Me</h2>
    <p>你好！我是一名来自<strong>中国科学技术大学</strong>的学生。</p>
    <p>我的研究方向是<strong>计算数学方向</strong>，技术兴趣包括算法、数据结构以及相关领域。</p>
    <p>在这里分享我的学习笔记、技术心得和生活感悟。</p>
</div>

<div class="section">
    <h2>Education</h2>
    <h3>中国科学技术大学</h3>
    <p>计算数学方向</p>
</div>

<div class="section">
    <h2>Research Interests</h2>
    <ul>
        <li>计算数学</li>
        <li>计算机辅助几何设计 (CAGD)</li>
        <li>计算机图形学</li>
        <li>机器学习与深度学习</li>
    </ul>
</div>

<div class="section">
    <h2>Skills</h2>
    <div>
        <span class="skill-tag">Python</span>
        <span class="skill-tag">C++</span>
        <span class="skill-tag">Git</span>
        <span class="skill-tag">VSCode</span>
        <span class="skill-tag">LaTeX</span>
        <span class="skill-tag">PyTorch</span>
    </div>
</div>

<div class="section">
    <h2>Contact</h2>
    <p>欢迎交流学习！</p>
    <div class="contact-row">
        <a href="https://github.com/ustc-zhengyi2023" class="contact-btn">
            💻 GitHub
        </a>
        <a href="mailto:zhengyi2023@mail.ustc.edu.cn" class="contact-btn">
            📧 Email
        </a>
    </div>
</div>
