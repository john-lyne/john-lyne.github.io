---
title: Spirituality Notes
layout: default
permalink: /booknotes/spirituality/
---

<h1>Spirituality Notes</h1>

<ul>
{% assign notes = site.booknotes | where: "category", "spirituality" | sort: "title" %}
{% for note in notes %}
  <li><a href="{{ note.url }}">{{ note.title }}</a> – {{ note.author }}</li>
{% endfor %}
</ul>
