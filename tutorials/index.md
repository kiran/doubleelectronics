---
layout: default
title: Tutorials
---

{% if site.tags.tutorial != empty %}
<ul class="posts">
  {% for post in site.tags.tutorial limit:3 %}
    <li><span>{{ post.date | date_to_string }}</span> <span class="seperator">~</span> <a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
{% endif %}