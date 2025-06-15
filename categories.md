---
title: "Kategori"
permalink: /categories/
layout: page
---
{% for category in site.categories %}
- [{{ category[0] }}]({{ "/categories/" | append: category[0] | relative_url }})
{% endfor %}

{% for category in site.categories %}
  <h2>{{ category | first }}</h2>
  <ul>
    {% for post in category.last %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

