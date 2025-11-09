---
layout: home
title: فادي الهرش
---
<h1>أهلاً وسهلاً في موقعي الأكاديمي</h1>
<p>باحث في <strong>Optimization & Machine Learning</strong><br>
مجموعة OML – KAUST</p>

<h2>آخر الأخبار والأوراق البحثية</h2>
<ul>
{% for post in site.posts limit:10 %}
  <li><strong>{{ post.date | date: '%Y-%m-%d' }}</strong> – <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>

<p><a href=\"/feed.xml\">RSS Feed</a> (للنشر التلقائي على تويتر/لينكدإن)</p>
