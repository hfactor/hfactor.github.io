---
layout: Post
permalink: /tags
title: Notes by Tags
content-type: static
---
{% assign tags =  site.notes | map: 'tags' | join: ','  | split: ',' | uniq %}
{% for tag in tags %}
  <h3 id="{{ tag }}">{{ tag }}</h3>
  <ul>
  {% for note in site.notes %}
    {% if note.tags contains tag and note.feed == "show" %}
    <li><a href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a></li>
    {% endif %}
  {% endfor %}
  </ul>
{% endfor %}