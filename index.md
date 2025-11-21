---
layout: default
title: Home
---

<div class="home-hero">
  <h1 class="hero-title">Marcus J. Davidson</h1>
  <p class="hero-subtitle">AI Platform Development | Digital Transformation | Strategic Advisory</p>
</div>

<div class="home-content">
  <section class="intro-section">
    <h2>Driving AI Industrialization at Scale</h2>
    <p>
      Strategic technology leader with proven impact across banking, private equity, and advisory sectors. 
      Currently spearheading ALAN, a core piece of DBS AI Industrialization efforts that enables governance 
      at scale across the enterprise, instrumental in DBS's recognition as the #1 Digital Bank (Euromoney 2023).
    </p>
    <p>
      Track record of delivering transformational outcomes: from closing $100M+ capital transactions and 
      managing $350M trading books to leading 600+ member technical communities. Expertise spans AI platform 
      development, digital transformation, financial markets, and strategic M&A—consistently translating 
      complex challenges into measurable business value.
    </p>
    <div class="cta-buttons">
      <a href="{{ '/about' | relative_url }}" class="btn btn-primary">View Full Experience</a>
      <a href="{{ '/posts' | relative_url }}" class="btn btn-secondary">Read My Posts</a>
    </div>
  </section>

  <section class="highlights">
    <h2>Core Expertise</h2>
    <div class="highlights-grid">
      <div class="highlight-item">
        <h3>Product & Program Leadership</h3>
        <p>Driving complex platforms and multi-release roadmaps end-to-end, ensuring delivery, adoption, and stakeholder alignment.</p>
      </div>
      <div class="highlight-item">
        <h3>Strategic Advisory & Commercial Strategy</h3>
        <p>Shaping growth strategies, investment theses, and M&A execution across sectors and markets.</p>
      </div>
      <div class="highlight-item">
        <h3>Stakeholder Influence & Executive Communication</h3>
        <p>Building trust across senior leaders, technical teams, and clients with clear, concise decision-ready communication.</p>
      </div>
      <div class="highlight-item">
        <h3>Data, Governance & Applied AI Enablement</h3>
        <p>Using analytical methods and practical AI implementation to improve workflows, enhance decision-making, and scale operational impact whilst balancing risk (regulatory & operational)</p>
      </div>
      <div class="highlight-item">
        <h3>Financial & Deal Structuring Expertise</h3>
        <p>Deep experience in valuation, capital raising, negotiations, and transaction management across PE, banking, and infrastructure.</p>
      </div>
      <div class="highlight-item">
        <h3>Cross-Functional Team Leadership</h3>
        <p>Leading diverse teams, managing priorities, and fostering high-engagement communities and collaborative cultures.</p>
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
