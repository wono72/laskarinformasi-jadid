---
title: "Tags"
permalink: /tags/
layout: page
---
{% for tag in site.tags %}
- [{{ tag[0] }}]({{ "/tags/" | append: tag[0] | relative_url }})
{% endfor %}

