---
layout: home
title: Fadi T. Elhersh
---

<h1>

<p>Computer Science Instructor @ Yanbu Industrial College</p>
<p>SCM Optimization & Machine Learning Researcher</p>
</h1>
<h2>Recent Posts</h2>

{% if site.posts.size > 0 -%}
<ul class="post-list">
  {% for post in site.posts limit:10 -%}
    <li>
      <strong>{{ post.date | date: '%d %b %Y' }}</strong> — <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      {% if post.excerpt and post.excerpt != empty -%}
        <br><small class="excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</small>
      {% endif %}
    </li>
  {% endfor -%}
</ul>
{% else -%}
<p>No posts yet. Check back soon!</p>
{% endif %}

<p><a href="{{ '/feed.xml' | relative_url }}">RSS Feed</a></p>
