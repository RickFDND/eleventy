---
title: My first page
layout: base.njk
templateEngineOverride: njk,md
---

## Blog Posts

{% for post in collections.posts %}
    {{ post.data.title }}
{% endfor %}

{% include "postlist.njk" %}

