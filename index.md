---
layout: home
title: فادي الهرش - موقع أكاديمي آلي
---
# أهلاً وسهلاً!

أنا **فادي الهرش**  
باحث في Optimization & Machine Learning  
KAUST – OML Research Group  

### آخر الأخبار والأوراق البحثية:
{% for post in site.posts limit:5 %}
- **{{ post.date | date: '%Y-%m-%d' }}** – [{{ post.title }}]({{ post.url }})
{% endfor %}

[جميع الأوراق البحثية]({{ '/feed.xml' | relative_url }})
