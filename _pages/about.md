---
permalink: /
title: "Francisco Patitucci"
excerpt: "Ph.D. student at UT Austin working on optimization for machine learning."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<p class="profile-lede">I am a Ph.D. student in the Department of Electrical and Computer Engineering at The University of Texas at Austin, advised by <a href="https://sites.utexas.edu/mokhtari/">Prof. Aryan Mokhtari</a>. I work on optimization for machine learning, with a focus on algorithms that are both theoretically principled and practically effective.</p>

<div class="profile-actions" aria-label="Primary links">
  <a class="btn btn--primary" href="/publications/">Publications</a>
  <a class="btn" href="/files/cv_Francisco_Patitucci_webpage.pdf">CV</a>
  <a class="btn" href="mailto:fpatitucci@utexas.edu">Email</a>
</div>

## Research Interests

<div class="research-grid">
  <section class="research-item">
    <h3>Optimization for Machine Learning</h3>
    <p>Algorithms with provable guarantees and strong empirical behavior in modern ML systems.</p>
  </section>
  <section class="research-item">
    <h3>Nonconvex Optimization</h3>
    <p>Methods for smooth nonconvex problems, including online-to-nonconvex conversion techniques.</p>
  </section>
  <section class="research-item">
    <h3>Adaptive and Online Methods</h3>
    <p>Online-learning-based optimization, adaptive optimizers, and quasi-Newton-inspired methods.</p>
  </section>
</div>

## Selected Publications

{% assign selected_publications = site.publications | sort: "date" | reverse %}
<div class="publication-list publication-list--compact">
{% for post in selected_publications limit: 2 %}
  <article class="publication-entry">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    {% if post.authors %}<p class="publication-authors">{{ post.authors }}</p>{% endif %}
    <p class="publication-venue"><em>{{ post.venue }}</em>, {{ post.date | date: "%Y" }}</p>
    {% if post.paperurl %}
      <p class="publication-links"><a class="btn btn--small" href="{{ post.paperurl }}">Paper</a></p>
    {% endif %}
  </article>
{% endfor %}
</div>

<p><a href="/publications/">View all publications</a> or visit my <a href="{{ site.author.googlescholar }}">Google Scholar profile</a>.</p>

## News

<ul class="news-list">
  <li><span class="news-date">2025</span><span>Paper on two-level online learning and quasi-Newton methods appeared at STOC 2025.</span></li>
  <li><span class="news-date">2025</span><span>New arXiv preprint on improving online-to-nonconvex conversion via double optimism.</span></li>
  <li><span class="news-date">2022</span><span>Received the Ing. Isidoro Marín Medal from the National Academy of Engineering of Argentina.</span></li>
</ul>

## Background

Before joining UT Austin, I earned my engineering degree from the Universidad Nacional de La Plata. I also pursued graduate studies in Mathematical Engineering at the Universidad de Buenos Aires.

I am open to internship opportunities in optimization, machine learning, and quantitative research.
