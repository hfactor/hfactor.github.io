---
layout: List
permalink: /tags
title: Movies
list-name: movie
content-type: static
---

<div>
    {% assign note_items = site.logs | reverse %}
    {% for note_items in note_items %}
        {%- if note_items.meta.type == page.list-name -%}
                <div class="notelist-feed">
                    <a href="{{ site.baseurl }}{{note_items.url}}">
                        {{note_items.title}}</a>, {{note_items.meta.language}} , {{note_items.meta.year}}, {{note_items.meta.rating}}
                </div>

        {%- endif -%}
    {%- endfor -%}
</div>
