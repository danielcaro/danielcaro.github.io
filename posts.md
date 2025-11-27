---
layout: page
title: Publicaciones
permalink: /posts/
---

## Lista de Publicaciones

{% for post in site.posts %}
- **[{{ post.title }}]({{ post.url | relative_url }})**  
  <small>{{ post.date | date: "%Y-%m-%d" }}</small>
{% endfor %}