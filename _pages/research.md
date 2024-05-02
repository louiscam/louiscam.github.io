---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
header:
  og_image: "research/ecdf.png"
---

My research falls into two main areas: developing new theory and methods in network data science, and leveraging statistics and network science to tackle complex biological problems using modern omics data. 

My theoretical work includes studying the optimal phase transition for global testing in the mixed membership stochastic block model and developing an [optimally adaptive global detection test]([https://projecteuclid.org/journals/bernoulli/volume-29/issue-3/Power-enhancement-and-phase-transitions-for-global-testing-of-the/10.3150/22-BEJ1519.short]). I also developed a new rate optimal algorithm for mixed membership estimation in dynamic networks under severe degree heterogeneity and temporal smoothness. The methods I design come with strong statistical guarantees and are applicable to, e.g., social networks and biological networks.

A large part of my methods work focuses on developing frameworks in computational biology. I developed a Python package to find [combinatorial markers](https://www.embopress.org/doi/full/10.15252/msb.20199005) for cell populations identified with single-cell RNA-seq data. In another work, I conceived a [drug repurposing pipeline](https://www.nature.com/articles/s41467-021-21056-z) to identify candidate drugs for repurposing against SARS-CoV-2. I also contributed to an [experimental design framework]([https://www.nature.com/articles/s42256-023-00719-0]) to better design _in vitro_ cell reprogramming experiments.

My applied work leverages statistics and network science to analyze modern genomic data sets in the context of cellular aging and nuclear mechanogenomics. I developed a novel [time-course approach]([https://onlinelibrary.wiley.com/doi/full/10.1111/acel.14056]) to identify age-associated transcription factors and investigated the coupling between gene transcription and spatial gene clustering in aging. I also characterized the [map]([https://www.biorxiv.org/content/10.1101/2023.12.07.570697v1]) between adhesome protein assemblies on the cell membrane and 3D organization of the corresponding genes in nucleus of IMR90 fibroblasts.
<nbsp>

{% include base_path %}

{% assign ordered_pages = site.research | sort:"order_number" %}

{% for post in ordered_pages %}
  {% include archive-single.html type="grid" %}
{% endfor %}
