---
layout: default
title: Techizz
permalink: /techizz/
---

<h2 style="font-size: 1.5rem; margin-bottom: 20px;">Techizz Articles</h2>

<div class="post-grid">
  {% for post in site.categories.techizz %}
    <a href="{{ post.url }}" style="text-decoration: none; color: inherit;">
      <div class="card">
        <img src="{{ post.image }}" class="card-img" alt="{{ post.title }}">
        <div class="card-content">
          <h3 class="card-title">{{ post.title }}</h3>
        </div>
      </div>
    </a>
  {% endfor %}
</div>