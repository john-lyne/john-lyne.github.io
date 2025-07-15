---
title: Poetry Notes
layout: default
permalink: /booknotes/poetry/
---

<h1>Poetry Notes</h1>

<ul>
{% assign notes = site.booknotes | where: "category", "poetry" | sort: "title" %}
{% for note in notes %}
  <li><a href="{{ note.url }}">{{ note.title }}</a> – {{ note.author }}</li>
{% endfor %}
</ul>
