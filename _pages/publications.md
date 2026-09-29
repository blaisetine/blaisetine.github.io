---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  You can also find my articles on <u><a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% assign pubs = site.publications | sort: "date" | reverse %}

## Conference & Journal Papers

{% for post in pubs %}{% if post.venue_type == "conference" or post.venue_type == "journal" %}
  {% include pub-item.html %}
{% endif %}{% endfor %}

## Workshop Papers

{% for post in pubs %}{% if post.venue_type == "workshop" %}
  {% include pub-item.html %}
{% endif %}{% endfor %}

## Posters

{% for post in pubs %}{% if post.venue_type == "poster" %}
  {% include pub-item.html %}
{% endif %}{% endfor %}

## Preprints

{% for post in pubs %}{% if post.venue_type == "preprint" %}
  {% include pub-item.html %}
{% endif %}{% endfor %}

## Patents

### Rasterization of compute shaders
A Glaister, BP Tine, D Sessions, M Lyapunov, Y Dotsenko

US Patent 9,529,575

### Vectorization of shaders
A Glaister, BP Tine, B Pelton, D Sessions, M Lyapunov, Y Dotsenko

US Patent 8,806,458

### Scalar optimizations for shaders
A Glaister, BP Tine, D Sessions, M Lyapunov, Y Dotsenko

US Patent 9,430,199

### Lookup tables for text rendering
BP Tine, CN Raubacher, AJR Hodsdon, MM Cohen

US Patent 9,129,441
