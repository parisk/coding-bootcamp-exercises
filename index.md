---
layout: default
---

## Presentations
<ul>
  <li><a href="{% link _presentations/javascript-p.html %}">JavaScript</a></li>
  <li><a href="{% link _presentations/react-p.html %}">React</a></li>
</ul>

## JavaScript exercises

<ul>
{% for doc in site.exercises %}
  <li><a href="{{ doc.url }}">{{ doc.title }}</a></li>
{% endfor %}
</ul>
