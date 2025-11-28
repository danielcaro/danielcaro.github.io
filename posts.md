---
layout: page
title: Posts
permalink: /posts/
---

<ul>
{% for tag in site.tags %}
  <li>
    <a href="/tag/{{ tag[0] | slugify }}/">
      {{ tag[0] }} ({{ tag[1].size }})
    </a>
  </li>
{% endfor %}
</ul>


{% for post in site.posts %}
- **[{{ post.title }}]({{ post.url | relative_url }})**  
  <small>{{ post.date | date: "%Y-%m-%d" }}</small>
{% endfor %}