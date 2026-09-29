---
layout: archive
title: "Open-Source Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

{% assign items = site.projects | sort: "date" | reverse %}
{% for post in items %}
  {% include archive-single.html %}
{% endfor %}