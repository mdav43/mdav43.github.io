---
layout: page
title: Posts
permalink: /posts/
---

<div class="posts-page">
  <h1>Blog Posts</h1>
  <p class="posts-intro">
    Thoughts, insights, and experiences from my professional journey in technology.
  </p>

  <div class="posts-list">
    {% if site.posts.size > 0 %}
      {% for post in site.posts %}
        <article class="post-item">
          <h2 class="post-title">
            <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          </h2>
          <p class="post-meta">
            <time datetime="{{ post.date | date_to_xmlschema }}">
              {{ post.date | date: "%B %d, %Y" }}
            </time>
            {% if post.categories.size > 0 %}
              • 
              {% for category in post.categories %}
                <span class="category">{{ category }}</span>
              {% endfor %}
            {% endif %}
          </p>
          <div class="post-excerpt">
            {{ post.excerpt }}
          </div>
          <a href="{{ post.url | relative_url }}" class="read-more">Read more →</a>
        </article>
      {% endfor %}
    {% else %}
      <p class="no-posts">No posts yet. Check back soon!</p>
    {% endif %}
  </div>
</div>
