---
layout: archive
title: "ORCAS Lab"
permalink: /lab/
author_profile: true
custom_header: true
---

<div class="lab-header">
  <img src="/images/orcas-logo.png" alt="ORCAS lab logo">
  <h1 class="page__title">ORCAS Lab</h1>
</div>

<img class="lab-hero" src="/images/orcas-banner.svg" alt="Vortex GPU architecture: the GPU core pipeline above a chip with GPU, CPU, and NPU">

The **Open-Source Research in Computer Architecture and Systems (ORCAS)** lab at UCLA builds open GPU hardware and software, and uses it to explore new GPU architectures for AI, graphics, and ray tracing. Our main platform is [Vortex](https://vortexgpgpu.github.io/), a full-stack, open-source RISC-V GPU. Students at every level, from first-year undergraduates to PhD candidates, make real research contributions on it.

## People

### Current Students

* Yanggon Kim
* Chengxuan Wang
* Nikhil Rout
* Jacob Leigh
* Xinle Song
* Mingxin Liu
* Pritam Mukhopadhyaya
{: .people-list}

### Former Students

* Kuan Fu Chen
* Mark Diaz
* Sagar Jain
* Brandon Kam
* Jacob Levinson
* Randall Liu
* Swastik Purathepparambil
* Injae Shin
* Michael Srouji
* Chenchen Tang
* Alex Tao
* Georgios Triantafyllou
* Nathan Wei
* Eliot Yoon
* Steve Zang
{: .people-list}

## Join ORCAS

We welcome students who want to build real hardware and software. If you are interested in GPU architecture, compilers, or open-source hardware, email me at [blaisetine@cs.ucla.edu](mailto:blaisetine@cs.ucla.edu) with your CV and a short note about what you would like to work on. Prospective PhD students should also apply to the [UCLA Computer Science PhD program](https://www.cs.ucla.edu/graduate-admissions/).

## Lab Publications

{% assign pubs = site.publications | where: "lab", "orcas" | sort: "date" | reverse %}
{% for post in pubs %}
  {% include pub-item.html %}
{% endfor %}
