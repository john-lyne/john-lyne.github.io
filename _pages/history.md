---
title: History Notes
layout: default
permalink: /booknotes/history/
---

<h1>History Notes</h1>

<ul>
{% assign notes = site.booknotes | where: "category", "history" | sort: "title" %}
{% for note in notes %}
  <li><a href="{{ note.url }}">{{ note.title }}</a> – {{ note.author }}</li>
{% endfor %}
</ul>
