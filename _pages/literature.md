---
title: Literature Notes
layout: default
permalink: /booknotes/literature/
---

<h1>Literature Notes</h1>

<ul>
{% assign notes = site.booknotes | where: "category", "literature" | sort: "title" %}
{% for note in notes %}
  <li><a href="{{ note.url }}">{{ note.title }}</a> – {{ note.author }}</li>
{% endfor %}
</ul>
