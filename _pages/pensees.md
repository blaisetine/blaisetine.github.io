---
layout: archive
title: "Pensées"
permalink: /pensees/
author_profile: false
---

Stories and reflections outside the lab, many of them written for curious kids.

{% assign items = site.pensees | sort: "date" | reverse %}
<div class="pensee-list">
{% for post in items %}
  <a class="pensee-card" href="{{ base_path }}{{ post.url }}">
    {% if post.image %}<img class="pensee-card__image" src="{{ base_path }}{{ post.image }}" alt="">{% endif %}
    <span class="pensee-card__body">
      <span class="pensee-card__title">{{ post.title }}</span>
      {% if post.subtitle %}<span class="pensee-card__subtitle">{{ post.subtitle }}</span>{% endif %}
      <span class="pensee-card__desc">{{ post.description }}</span>
      <span class="pensee-card__date">{{ post.date | date: "%B %Y" }}</span>
    </span>
  </a>
{% endfor %}
</div>

<p class="pensees-note">Personal writing. Views are my own, not UCLA's.</p>
