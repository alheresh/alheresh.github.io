---
layout: home
title: Fadi T. Elhersh
---
<h1>Fadi T. Elhersh</h1>
<p> Computer Science Instructor @ Yanbu Industrial College </p>
<p> SCM Optimization & Machine Learning Researcher </p>
<url>
{% for post in site.posts limit:10 %}
  <li><strong>{{ post.date | date: '%Y-%m-%d' }}</strong> – <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>

<p><a href=\"/feed.xml\">RSS Feed</a> </p>
