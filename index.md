---
layout: default
---

## JavaScript exercises

<ul>
{% for doc in site.exercises %}
    <li><a href="{{ doc.url }}">{{ doc.title }}</a></li>
{% endfor %}
</ul>
