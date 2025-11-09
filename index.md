---
layout: home
title: Fadi T. Elhersh
---

<header class="home-header">
  <h1>{{ page.title }}</h1>
  
  <p class="subtitle">
    **Computer Science Instructor** @ Yanbu Industrial College
    <br>
    SCM Optimization & **Machine Learning Researcher**
  </p>
</header>

<hr>

<h2>Recent Posts</h2>

{% if site.posts.size > 0 -%}
<ul class="post-list">
  {% for post in site.posts limit:10 -%}
    <li>
      <span class="post-date">{{ post.date | date: '%d %b %Y' }}</span> — 
      <a href="{{ post.url | relative_url }}" class="post-link">{{ post.title }}</a>
      
      {% if post.excerpt and post.excerpt != empty -%}
        <p class="excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>
      {% endif %}
    </li>
  {% endfor -%}
</ul>
{% else -%}
<p>No posts yet. Check back soon!</p>
{% endif %}

<p class="rss-link"><a href="{{ '/feed.xml' | relative_url }}">RSS Feed</a></p>
