---
layout: default
title: Home
---

<div class="home-hero">
  <h1 class="hero-title">Welcome to My Professional Portfolio</h1>
  <p class="hero-subtitle">Technology Professional | Developer | Problem Solver</p>
</div>

<div class="home-content">
  <section class="intro-section">
    <h2>Hello, I'm [Your Name]</h2>
    <p>
      I'm a passionate technology professional with expertise in software development, 
      problem-solving, and delivering innovative solutions. This site showcases my 
      professional journey, experiences, and insights.
    </p>
    <div class="cta-buttons">
      <a href="{{ '/about' | relative_url }}" class="btn btn-primary">About Me</a>
      <a href="{{ '/posts' | relative_url }}" class="btn btn-secondary">Read My Posts</a>
    </div>
  </section>

  <section class="highlights">
    <h2>What I Do</h2>
    <div class="highlights-grid">
      <div class="highlight-item">
        <h3>💻 Development</h3>
        <p>Building scalable and efficient software solutions</p>
      </div>
      <div class="highlight-item">
        <h3>🚀 Innovation</h3>
        <p>Exploring new technologies and best practices</p>
      </div>
      <div class="highlight-item">
        <h3>📚 Learning</h3>
        <p>Continuous growth and knowledge sharing</p>
      </div>
    </div>
  </section>

  <section class="recent-posts">
    <h2>Latest Posts</h2>
    <div class="posts-list">
      {% for post in site.posts limit:3 %}
        <article class="post-preview">
          <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
          <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
          <p>{{ post.excerpt }}</p>
        </article>
      {% endfor %}
    </div>
    <a href="{{ '/posts' | relative_url }}" class="view-all-link">View all posts →</a>
  </section>
</div>
