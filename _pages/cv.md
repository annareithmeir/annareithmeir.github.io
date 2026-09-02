---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
---

{% include base_path %}

<!--
  TODO (Anna): a few fields below are placeholders because they weren't
  in the existing site content — please fill in / correct before this goes live:
    - Exact PhD start date
    - B.Sc. / M.Sc. graduation years
    - Skills section (languages, frameworks, tools) is empty on purpose
    - Add a "Talks" or "Awards" entry if there's more than the SPIE finalist
-->

<p class="cv-intro">PhD student in Informatics, working on data-driven models for medical image registration. Advised by Prof. Julia Schnabel at the <a href="https://compai-lab.github.io/">Chair of Computational Imaging and AI in Medicine</a>, TU Munich.</p>

<div class="cv-section">
  <h2 class="cv-section__title">Education</h2>

  <div class="cv-entry">
    <span class="cv-entry__date">20XX&ndash;Present</span>
    <div>
      <h3 class="cv-entry__title">Ph.D. in Informatics</h3>
      <p class="cv-entry__subtitle">Technical University of Munich &mdash; Chair of Computational Imaging and AI in Medicine</p>
      <p class="cv-entry__detail">Advisor: Prof. Julia A. Schnabel. Research on data-driven, physics-inspired regularization and Riemannian manifolds for medical image registration.</p>
    </div>
  </div>

  <div class="cv-entry">
    <span class="cv-entry__date">20XX</span>
    <div>
      <h3 class="cv-entry__title">M.Sc. in Informatics</h3>
      <p class="cv-entry__subtitle">Technical University of Munich</p>
      <p class="cv-entry__detail">Focus on computer vision and high-performance computing.</p>
    </div>
  </div>

  <div class="cv-entry">
    <span class="cv-entry__date">20XX</span>
    <div>
      <h3 class="cv-entry__title">B.Sc. in Informatics</h3>
      <p class="cv-entry__subtitle">Technical University of Munich</p>
    </div>
  </div>
</div>

<div class="cv-section">
  <h2 class="cv-section__title">Selected Publications</h2>
  {% assign pubs = site.publications | sort: 'date' | reverse %}
  {% for post in pubs %}
    {% if post.id %}
      {% assign pub_title = post.title | markdownify | remove: "<p>" | remove: "</p>" %}
    {% else %}
      {% assign pub_title = post.title %}
    {% endif %}
    <div class="cv-entry">
      <span class="cv-entry__date">{{ post.date | default: "1900-01-01" | date: "%Y" }}</span>
      <div>
        <h3 class="cv-entry__title"><a href="{{ base_path }}{{ post.url }}">{{ pub_title }}</a></h3>
        <p class="cv-entry__subtitle">{{ post.venue }}</p>
      </div>
    </div>
  {% endfor %}
  <p class="cv-entry__detail"><a href="{{ '/publications/' | relative_url }}">Full list with abstracts &amp; links &rarr;</a></p>
</div>

<div class="cv-section">
  <h2 class="cv-section__title">Awards &amp; Honors</h2>
  <div class="cv-entry">
    <span class="cv-entry__date">2024</span>
    <div>
      <h3 class="cv-entry__title">Finalist, Robert F. Wagner Award</h3>
      <p class="cv-entry__subtitle">SPIE Medical Imaging 2024</p>
    </div>
  </div>
</div>

<div class="cv-section">
  <h2 class="cv-section__title">Teaching</h2>
  <div class="cv-entry">
    <span class="cv-entry__date">WS23</span>
    <div>
      <h3 class="cv-entry__title">Master&rsquo;s Seminar: Learning of and on Manifolds in Medical Imaging</h3>
      <p class="cv-entry__subtitle">TU Munich</p>
    </div>
  </div>
  <div class="cv-entry">
    <span class="cv-entry__date"></span>
    <div>
      <h3 class="cv-entry__title">Outreach workshops</h3>
      <p class="cv-entry__detail">Girls&rsquo; Day and further high-school workshops (with the Munich Center for Machine Learning); workshop for Bavarian informatics high-school teachers (with the TU Munich Computing Education Research Group).</p>
    </div>
  </div>
  <p class="cv-entry__detail">See the <a href="{{ '/teaching/' | relative_url }}">Teaching page</a> for more.</p>
</div>

<div class="cv-section">
  <h2 class="cv-section__title">Skills</h2>
  <p class="cv-entry__detail"><!-- TODO (Anna): list languages, frameworks, and tools here, e.g. Python, PyTorch, C++, HPC/SLURM --></p>
</div>
