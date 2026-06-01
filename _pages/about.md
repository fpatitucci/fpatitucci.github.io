---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a Ph.D. student in the Department of Electrical and Computer Engineering at The University of Texas at Austin, advised by [Prof. Aryan Mokhtari](https://sites.utexas.edu/mokhtari/). I work on optimization for machine learning, with a focus on algorithms that are both theoretically principled and practically effective. Recently, my work has explored nonconvex optimization, online-learning-based methods, and adaptive optimizers.

I am also open to internship opportunities in optimization, machine learning, and quantitative research.

Before joining UT Austin, I earned my engineering degree from the Universidad Nacional de La Plata, where I received the 2022 Ing. Isidoro Marín Medal from the National Academy of Engineering of Argentina. I also pursued graduate studies in Mathematical Engineering at the Universidad de Buenos Aires.

## Publications

For a complete list see my [Google Scholar profile]({{ site.author.googlescholar }}).

{% assign publications = site.publications | sort: "date" | reverse %}
<div class="publication-list">
{% for post in publications %}
  <article class="publication-entry">
    <h3>{{ post.title }}</h3>
    {% if post.authors %}<p class="publication-authors">{{ post.authors }}</p>{% endif %}
    <p class="publication-venue"><em>{{ post.venue }}</em>, {{ post.date | date: "%Y" }}</p>
    {% if post.paperurl %}
      <p class="publication-links"><a href="{{ post.paperurl }}">Paper</a></p>
    {% endif %}
  </article>
{% endfor %}
</div>
