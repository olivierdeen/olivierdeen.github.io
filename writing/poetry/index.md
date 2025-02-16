---
layout: page 
title: Poetry
---

<div class="poetry-section">
  <header class="poetry-header">
    <p class="poetry-intro">These are my attempts at poems — explorations in verse and rhythm.</p>
  </header>

  <div class="poetry-grid">
    {% for post in site.categories.poetry %}
      <article class="poetry-tile">
        <a href="{{ post.url }}" class="poetry-tile-link">
          <h2 class="poetry-tile-title">{{ post.title }}</h2>
          <time class="poetry-tile-date" datetime="{{ post.date | date_to_xmlschema }}">
            {{ post.date | date: "%B %d, %Y" }}
          </time>
        </a>
      </article>
    {% endfor %}
  </div>
</div>



