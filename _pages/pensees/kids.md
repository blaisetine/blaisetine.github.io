---
layout: archive
title: "For Curious Kids"
permalink: /pensees/kids/
author_profile: false
section: kids
---

{% assign section = site.data.pensees | where: "id", page.section | first %}
{{ section.description }}

{% assign items = site.pensees | where: "section", page.section | sort: "date" | reverse %}
<div class="pensee-list">
{% for post in items %}
  {% include pensee-card.html full=true %}
{% endfor %}
</div>

<p class="pensees-back"><a href="{{ base_path }}/pensees/">&larr; All Pensées</a></p>
