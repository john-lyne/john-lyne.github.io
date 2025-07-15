---
title: Science Notes
layout: default
permalink: /booknotes/science/
---

<h1>Science Notes</h1>

<ul>
{% assign notes = site.booknotes | where: "category", "science" | sort: "title" %}
{% for note in notes %}
  <li><a href="{{ note.url }}">{{ note.title }}</a> – {{ note.author }}</li>
{% endfor %}
</ul>
