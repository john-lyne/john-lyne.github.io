---
title: Philosophy Notes
layout: default
permalink: /booknotes/philosophy/
---

<h1>Philosophy Notes</h1>

<ul>
{% assign notes = site.booknotes | where: "category", "philosophy" | sort: "title" %}
{% for note in notes %}
  <li><a href="{{ note.url }}">{{ note.title }}</a> – {{ note.author }}</li>
{% endfor %}
</ul>
