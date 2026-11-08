---
layout: page
title: Tags
permalink: /tags/
---

<ul>
{% for tag in site.tags %}
    {% assign tag_slug = tag[0] | slugify %}
    <li>
        <a href="{{ '/tags/' | append: tag_slug | append: '/' | relative_url }}">{{ tag[0] }}</a>
        <span>({{ tag[1] | size }})</span>
    </li>
{% endfor %}
</ul>
