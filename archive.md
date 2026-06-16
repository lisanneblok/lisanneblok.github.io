---
layout: page
title: Blog Archive
---

{%- assign all_keywords = site.posts | map: "keywords" | flatten | uniq | sort -%}

{% for keyword in all_keywords %}
  <h3 id="{{ keyword | slugify }}">{{ keyword }}</h3>
  <ul>
    {% for post in site.posts %}
      {% if post.keywords contains keyword %}
        <li><a href="{{ post.url }}">{{ post.date | date: "%B %Y" }} — {{ post.title }}</a></li>
      {% endif %}
    {% endfor %}
  </ul>
{% endfor %}
