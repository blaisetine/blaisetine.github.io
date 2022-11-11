---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

## Patents

### Rasterization of compute shaders
A Glaister, BP Tine, D Sessions, M Lyapunov, Y Dotsenko

US Patent 9,529,575

### Vectorization of shaders
A Glaister, BP Tine, B Pelton, D Sessions, M Lyapunov, Y Dotsenko

US Patent 8,806,458	11	2014

### Scalar optimizations for shaders
A Glaister, BP Tine, D Sessions, M Lyapunov, Y Dotsenko

US Patent 9,430,199

### Lookup tables for text rendering
BPF Tine, CN Raubacher, AJR Hodsdon, MM Cohen

US Patent 9,129,441