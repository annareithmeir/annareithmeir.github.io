---
title: "From Model Based to Learned Regularization in Medical Image Registration: A Comprehensive Review"
collection: publications
permalink: /publication/2026-media-review
date: 2026-01-01
venue: 'Medical Image Analysis'
arxiv: 'https://arxiv.org/abs/2412.15740'
code: 'https://github.com/annareithmeir/regularization-in-medical-image-registration'
authors: '<b>Anna Reithmeir</b>, Veronika Spieker, Vasiliki Sideri-Lampretsa, Daniel Rueckert, Julia A. Schnabel, Veronika A. Zimmer'
bibtex: false
---

{{ page.authors }}

## Abstract

> Image registration is fundamental in medical imaging applications, such as disease progression analysis or radiation therapy planning. The primary objective of image registration is to precisely capture the deformation between two or more images, typically achieved by minimizing an optimization problem. Due to its inherent ill-posedness, regularization is a key component in driving the solution toward anatomically meaningful deformations. A wide range of regularization methods has been proposed for both conventional and deep learning-based registration. However, the appropriate application of regularization techniques often depends on the specific registration problem, and no one-fits-all method exists. Despite its importance, regularization is often overlooked or addressed with default approaches, assuming existing methods are sufficient. A comprehensive and structured review remains missing. This review addresses this gap by introducing a novel taxonomy that systematically categorizes the diverse range of proposed regularization methods. It highlights the emerging field of learned regularization, which leverages data-driven techniques to automatically derive deformation properties from the data. Moreover, this review examines the transfer of regularization methods from conventional to learning-based registration, identifies open challenges, and outlines future research directions. By emphasizing the critical role of regularization in image registration, we hope to inspire the research community to reconsider regularization strategies in modern registration algorithms and to explore this rapidly evolving field further.

## Resources

{% if page.paperurl %}<a href=" {{ page.paperurl }} ">[pdf]</a>{% endif %} {% if page.arxiv %}<a href=" {{ page.arxiv }} ">[arxiv]</a>{% endif %} {% if page.code %}<a href=" {{ page.code }} ">[github]</a>{% endif %} {% if page.video %}<a href=" {{ page.video }} ">[video]</a>{% endif %} {% if poster %}<a href=" {{ page.poster }} ">[video]</a>{% endif %}
