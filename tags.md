---
layout: page
title: Tags
permalink: /tags/
---

<ul>
{% for tag in site.tags %}
    <li><a href="{{ '/tags/' | append: tag[0] | slugify | append: '/' | relative_url }}">{{ tag[0] }}</a></li>
{% endfor %}
</ul>
