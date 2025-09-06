---
layout: default
title: Inicio
description: Últimos artículos
---

# Últimos artículos

{% for post in site.posts limit: 10 %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%-d %b %Y" }}
{% endfor %}
