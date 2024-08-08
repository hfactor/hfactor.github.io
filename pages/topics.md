---
title: Topics
layout: Static
cat-value: Topics
permalink: /Topics
---
<div class="slot-medium">
{% assign sorted_notes = site.notes | sort: 'category-order' %}
{% assign first_item = true %}
  {% for note_page in sorted_notes %}
    {% if note_page.category == "MOC" %}
      {% assign count = 0 %}
      {% for note in site.notes %}
        {% if note.category == note_page.cat-value %}
          {% assign count = count | plus: 1 %}
        {% endif %}
      {% endfor %}
      {% if count > 0 %}
        {% if first_item %}
          {% assign first_item = false %}
        {% else %},
        {% endif %}
      <a href="{{ note_page.url }}">{{note_page.title}}</a><sup>{{count}}</sup>
      {% endif %}
    {% endif %}
  {% endfor %}
  </div>

<div class="slot-large">
<h2>Latest Notes</h2>
<div class="note-list-sec">
    <ul class="note-list"> 
      {% assign non_moc_notes = site.notes | where_exp: "note", "note.category != 'MOC'" %}
      {% assign sorted_notes = non_moc_notes | sort: 'date' | reverse %}
      {% assign latest_notes = sorted_notes | slice: 0, 30 %}
      {% for note in latest_notes %}
          <li>
              <a href="{{ note.url }}">{{ note.title }}</a>
          </li>
      {% endfor %}
    </ul>
    </div> </div>