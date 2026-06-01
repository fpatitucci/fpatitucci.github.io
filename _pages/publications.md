---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

This page collects my research papers. You can also find an automatically updated list on my <a href="{{ site.author.googlescholar }}">Google Scholar profile</a>.

{% assign publications = site.publications | sort: "date" | reverse %}
<div class="publication-list">
{% for post in publications %}
  <article class="publication-entry">
    <h2>{{ post.title }}</h2>
    {% if post.authors %}<p class="publication-authors">{{ post.authors }}</p>{% endif %}
    <p class="publication-venue"><em>{{ post.venue }}</em>, {{ post.date | date: "%Y" }}</p>
    {% if post.paperurl %}
      <p class="publication-links"><a href="{{ post.paperurl }}">Paper</a></p>
    {% endif %}
  </article>
{% endfor %}
</div>

{% if publications.size == 0 %}
  <p>No publications have been added yet.</p>
{% endif %}
