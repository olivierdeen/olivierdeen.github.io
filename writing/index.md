---
layout: default
title: Writing
---

# Writing Section
Welcome to the storage place for the ramblings of my mind.

<div class="writing-grid">
{% for post in site.categories.thought %}
    <article class="writing-tile">
    <a href="{{ post.url }}" class="writing-tile-link">
        <h2 class="writing-tile-title">{{ post.title }}</h2>
        <time class="writing-tile-date" datetime="{{ post.date | date_to_xmlschema }}">
        {{ post.date | date: "%B %d, %Y" }}
        </time>
    </a>
    </article>
{% endfor %}
</div>