---
title: "Covariance Descriptors Meet General Vision Encoders: Riemannian Deep Learning for Medical Image Classification"
collection: publications
permalink: /publication/2026-isbi
date: 2026-02-01
venue: 'Submitted to IEEE ISBI 2026'
arxiv: 'https://arxiv.org/abs/2511.04190'
code: 'https://github.com/compai-lab/2026-isbi-mayr'
authors: 'Josef Mayr, <b>Anna Reithmeir</b>, Maxime Di Folco, Julia A. Schnabel'
bibtex: false
---

{{ page.authors }}

## Abstract

> Covariance descriptors capture second-order statistics of image features. They have shown strong performance in general computer vision tasks, but remain underexplored in medical imaging. We investigate their effectiveness for both conventional and learning-based medical image classification, with a particular focus on SPDNet, a classification network specifically designed for symmetric positive definite (SPD) matrices. We propose constructing covariance descriptors from features extracted by pre-trained general vision encoders (GVEs) and comparing them with handcrafted descriptors. Two GVEs - DINOv2 and MedSAM - are evaluated across eleven binary and multi-class datasets from the MedMNSIT benchmark. Our results show that covariance descriptors derived from GVE features consistently outperform those derived from handcrafted features. Moreover, SPDNet yields superior performance to state-of-the-art methods when combined with DINOv2 features. Our findings highlight the potential of combining covariance descriptors with powerful pretrained vision encoders for medical image analysis.

## Resources

{% if page.paperurl %}<a href=" {{ page.paperurl }} ">[pdf]</a>{% endif %} {% if page.arxiv %}<a href=" {{ page.arxiv }} ">[arxiv]</a>{% endif %} {% if page.code %}<a href=" {{ page.code }} ">[github]</a>{% endif %} {% if page.video %}<a href=" {{ page.video }} ">[video]</a>{% endif %} {% if poster %}<a href=" {{ page.poster }} ">[video]</a>{% endif %}
