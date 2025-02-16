---
layout: default
title: Poetry
---

# Poetry Section
These my attempts at poems

# Poetry Collection

{% for post in site.categories.poetry %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

