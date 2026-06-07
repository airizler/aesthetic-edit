---
layout: default
title: Home Decor, Dining & DIY
permalink: /home-decor-dining-diy/
---

<div style="margin-bottom: 40px; text-align: center;">
  <h1 style="font-size: 2.5rem; margin-bottom: 15px;">Home Decor, Dining & DIY</h1>
  <p style="color: var(--text-muted); font-size: 1.1rem;">Explore beautiful home organization hacks and dining aesthetics.</p>
</div>

<div class="post-grid">
  {% for post in site.categories["Home Decor Dining DIY"] %}
  <a href="{{ post.url }}" style="text-decoration: none; color: inherit;">
    <div class="card">
      <img src="{{ post.image }}" class="card-img" alt="{{ post.title }}">
      <div class="card-content">
        <p class="card-category">{{ post.categories | first }}</p>
        <h3 class="card-title">{{ post.title }}</h3>
        <p style="color: var(--text-muted); font-size: 0.9rem; margin-top: 10px;">{{ post.excerpt | strip_html | truncatewords: 15 }}</p>
      </div>
    </div>
  </a>
  {% endfor %}
</div>