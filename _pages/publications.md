---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

<p class="cv-intro">You can also find my articles on <a href="https://scholar.google.com/citations?hl=de&user=RjjBUtEAAAAJ">my Google Scholar profile</a>.</p>

{% assign pubs = site.publications | sort: 'date' | reverse %}
{% assign current_year = "" %}
{% for post in pubs %}
  {% assign this_year = post.date | default: "1900-01-01" | date: "%Y" %}
  {% if this_year != current_year %}
    <h2 class="home-section__title" style="margin: 2em 0 1em;">{{ this_year }}</h2>
    {% assign current_year = this_year %}
  {% endif %}
  {% if post.id %}
    {% assign pub_title = post.title | markdownify | remove: "<p>" | remove: "</p>" %}
  {% else %}
    {% assign pub_title = post.title %}
  {% endif %}
  <article class="pub-card" style="margin-bottom: 1em;">
    {% if post.teaser %}
      <img class="pub-card__teaser" src="{{ post.teaser | prepend: '/images' | prepend: base_path }}" alt="" />
    {% endif %}
    <div>
      <div class="pub-card__meta">
        <span class="pub-card__venue">{{ post.venue }}</span>
        <span class="pub-card__year">{{ this_year }}</span>
      </div>
      <h3 class="pub-card__title"><a href="{{ base_path }}{{ post.url }}">{{ pub_title }}</a></h3>
      <p class="pub-card__authors">{{ post.authors }}</p>
      <div class="pub-card__links">
        {% if post.arxiv %}<a href="{{ post.arxiv }}">arXiv</a>{% endif %}
        {% if post.code %}<a href="{{ post.code }}">Code</a>{% endif %}
        {% if post.paperurl %}<a href="{{ post.paperurl }}">PDF</a>{% endif %}
        {% if post.video %}<a href="{{ post.video }}">Video</a>{% endif %}
        {% if post.poster %}<a href="{{ post.poster }}">Poster</a>{% endif %}
        <a href="{{ base_path }}{{ post.url }}">Abstract &rarr;</a>
      </div>
    </div>
  </article>
{% endfor %}
