---
layout: page
title: Blog
permalink: /posts/
---

<script>
window.MathJax = {
  loader: {load: ['input/tex', 'output/chtml']},
  tex: {
    inlineMath: [['$', '$']],
    displayMath: [['$$', '$$']]
  }
};
</script>
<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-svg.js" async></script>

<style>
.page-content {
    max-width: 900px;
    margin: 0 auto;
    padding: 40px 20px;
}
.hero {
    text-align: center;
    padding: 50px 30px;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    border-radius: 20px;
    margin-bottom: 40px;
    box-shadow: 0 10px 40px rgba(102, 126, 234, 0.3);
}
.hero h1 {
    font-size: 2.5em;
    color: #fff;
    margin-bottom: 10px;
}
.hero p {
    color: rgba(255, 255, 255, 0.9);
    font-size: 1.1em;
}
.post-card {
    background: #fff;
    border-radius: 16px;
    padding: 30px;
    margin-bottom: 25px;
    border: 1px solid rgba(0, 0, 0, 0.08);
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.05);
    transition: all 0.3s ease;
}
.post-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 30px rgba(0, 0, 0, 0.1);
}
.post-header {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    margin-bottom: 15px;
}
.post-title {
    font-size: 1.4em;
    color: #2d3748;
    text-decoration: none;
    font-weight: 600;
    transition: color 0.3s ease;
}
.post-title:hover {
    color: #667eea;
}
.post-date {
    color: #8896a6;
    font-size: 0.9em;
    font-family: "SF Mono", Monaco, monospace;
}
.post-excerpt {
    color: #555;
    line-height: 1.8;
    margin-bottom: 15px;
}
.post-tags {
    display: flex;
    gap: 8px;
    flex-wrap: wrap;
}
.post-tag {
    padding: 4px 12px;
    background: #f7fafc;
    color: #667eea;
    border-radius: 15px;
    font-size: 0.85em;
}
.read-more {
    display: inline-block;
    padding: 10px 25px;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: #fff !important;
    text-decoration: none;
    border-radius: 20px;
    font-weight: 500;
    transition: all 0.3s ease;
    margin-top: 10px;
}
.read-more:hover {
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
.empty-state {
    text-align: center;
    padding: 60px 30px;
    background: #fff;
    border-radius: 16px;
    color: #8896a6;
}
</style>

<a href="/" class="back-link">← Back to Home</a>

<div class="hero">
    <h1>Blog</h1>
    <p>学习笔记、技术分享与生活感悟</p>
</div>

{% for post in site.posts %}
<div class="post-card">
    <div class="post-header">
        <a href="{{ post.url }}" class="post-title">{{ post.title }}</a>
        <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
    </div>
    {% if post.excerpt %}
    <div class="post-excerpt">{{ post.excerpt }}</div>
    {% endif %}
    <div class="post-tags">
        <span class="post-tag">{{ post.categories }}</span>
    </div>
    <a href="{{ post.url }}" class="read-more">Read More →</a>
</div>
{% endfor %}

{% if site.posts.size == 0 %}
<div class="empty-state">
    <p style="font-size: 1.2em;">📝 博客正在建设中...</p>
    <p>内容即将上线，敬请期待！</p>
</div>
{% endif %}
