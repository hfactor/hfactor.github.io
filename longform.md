---
layout: post
title: Longform Working Notes
permalink: /longform
content-type: eg
---

<main>
    {%- for item in site.notes -%}
    {%- if item.notetype == "longform" -%}
    <div class="feed-title-excerpt-block disable-select" data-url="{{site.url}}{{item.url}}">
        <a href="{{item.url}}" style="text-decoration: none; color: #333333;">
        <p class="feed-title">{{ item.title }}</p>
        </a>
    </div>
    {%- endif -%}
    {%- endfor -%}
</main>
