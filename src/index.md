---
title: My first page
layout: base.njk
---

## Blog Posts

{% for post in collections.posts %}
    {{ post.data.title }}
{% endfor %}

<ul>
    {% for post in collections.posts %}
    <li><a href="{{ post.url }}">{{ post.data.title }}</a></li>
    {% endfor %}
</ul>
