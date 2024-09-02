---
permalink: /
title: ""
excerpt: "Anna Reithmeir - PhD Student at the University of Munich - Chair for Computational Imaging and AI in Medicine"
author_profile: true
redirect_from:
  - /about/
---

Anna Reithmeir is a PhD student at the [Chair of Computational Imaging and AI in Medicine](https://compai-lab.github.io/) at TU Munich under the supervision of Prof. Julia Schnabel. She received her B.Sc. and M.Sc. in Informatics from TU Munich with a focus on computer vision and high performance computing. 

Her research interests lie in data-driven models for medical image registration, physics-inspired regularization, and Riemannian manifolds.


News
======
  <ul>{% assign items = site.news | sort: 'date' | reverse %}
{% for post in items limit:5 %}
    {% include archive-news.html %}
  {% endfor %}</ul>
