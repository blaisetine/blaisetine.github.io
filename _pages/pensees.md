---
layout: archive
title: "Pensées"
permalink: /pensees/
author_profile: false
---

Stories and reflections outside the lab: science for curious kids, things I build, and thoughts on Africa and painting.

{% for section in site.data.pensees %}
{% assign items = site.pensees | where: "section", section.id | sort: "date" | reverse %}
{% if items.size > 0 %}
<section class="pensee-section">
  <h2 class="pensee-section__title"><a href="{{ base_path }}/pensees/{{ section.id }}/">{{ section.title }}</a></h2>
  <p class="pensee-section__desc">{{ section.description }}</p>
  <div class="pensee-grid">
  {% for post in items limit: 3 %}
    {% include pensee-card.html %}
  {% endfor %}
  </div>
  <p class="pensee-section__more"><a href="{{ base_path }}/pensees/{{ section.id }}/">All {{ section.title }} ({{ items.size }}) &rarr;</a></p>
</section>
{% endif %}
{% endfor %}

<p class="pensees-note">Personal writing. Views are my own, not UCLA's.</p>
