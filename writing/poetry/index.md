---
layout: page 
title: Poetry
---

<div class="poetry-section">
  <header class="poetry-header">
    <h1>Poetry Collection</h1>
    <p class="poetry-intro">These are my attempts at poems — explorations in verse and rhythm.</p>
  </header>
    
  <div class="poetry-styles">
    <h2>Poetry Styles</h2>
    <ul>
      <li>
        <strong>Dierenversjes/Animal Poems</strong> - Inspired by the works of the Dutch poet Kees Stip, who wrote poems under the pseudonym Trijntje Fop. These poems are characterized by their anthropomorphising of animals in the spirit of Aesopus and La Fontaine, a reference to a location on the first line and wordplay and puns. Originally the style has a strict rhyme scheme and meter, but while I try to keep the rhyme scheme, I do not attempt to keep the meter.
      </li>
      <li>
        <strong>Haikus</strong> - Three lines of five, seven, and five syllables respectively. 
      </li>
      <li>
        <strong>Free Verse</strong> - Any other style of poem that does not fit the above forms.
      </li>
    </ul>
  </div>

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



