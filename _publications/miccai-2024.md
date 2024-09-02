---
title: "Data-Driven Tissue-and Subject-Specific Elastic Regularization for Medical Image Registration"
collection: publications
permalink: /publication/2024-miccai
date: 2024-03-01
venue: 'MICCAI 2024'
arxiv: 'https://arxiv.org/abs/2407.04355'
code: 'github.com/compai-lab/2024-miccai-koegl'
authors: '<b>Anna Reithmeir</b>, Lina Felsner, Rickmer Braren, Julia A. Schnabel, Veronika A. Zimmer'
teaser: /previews/miccai-2024.png
bibtex: false
---

{{ page.authors }}

<img class="pub_teaser" src="../images/previews/miccai-2024.png" alt="Teaser Image" title="teaser" />

## Abstract

> Physics-inspired regularization is desired for intra-patient image registration since it can effectively capture the biomechanical characteristics of anatomical structures. However, a major challenge lies in the reliance on physical parameters: Parameter estimations vary widely across the literature, and the physical properties themselves are inherently subject-specific. In this work, we introduce a novel data-driven method that leverages hypernetworks to learn the tissue-dependent elasticity parameters of an elastic regularizer. Notably, our approach facilitates the estimation of patient-specific parameters without the need to retrain the network. We evaluate our method on three publicly available 2D and 3D lung CT and cardiac MR datasets. We find that with our proposed subject-specific tissue-dependent regularization, a higher registration quality is achieved across all datasets compared to using a global regularizer. The code is available at [https://github.com/compai-lab/2024-miccai-reithmeir](https://github.com/compai-lab/2024-miccai-reithmeir).

## Resources

{% if page.paperurl %}<a href=" {{ page.paperurl }} ">[pdf]</a>{% endif %} {% if page.arxiv %}<a href=" {{ page.arxiv }} ">[arxiv]</a>{% endif %} {% if page.code %}<a href=" {{ page.code }} ">[github]</a>{% endif %} {% if page.video %}<a href=" {{ page.video }} ">[video]</a>{% endif %} {% if poster %}<a href=" {{ page.poster }} ">[video]</a>{% endif %}

