---
layout: page
title: Posts
permalink: /posts/
---


{% for tag in site.tags %}
    `[{{ tag[0] }} ({{ tag[1].size }})](/tags/{{ tag[0] | slugify }}/)`
{% endfor %}

---

{% for post in site.posts %}
- **[{{ post.title }}]({{ post.url | relative_url }})**  
  <small>{{ post.date | date: "%Y-%m-%d" }}</small>
{% endfor %}