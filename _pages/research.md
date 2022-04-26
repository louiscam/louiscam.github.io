---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
header:
  og_image: "research/ecdf.png"
---

My research falls into two main areas: developing new methods and theory in network systems, and addressing complex biological problems using machine learning on modern omics data. One strand of research in this first area develops a [novel hypothesis test](https://arxiv.org/abs/2204.11109) for detecting the presence of communities in networks in which agents can simultaneously belong to several communities. My interest in time-evolving systems also informs a current project on the estimation of mixed memberships in dynamic network. The methods I design come with strong statistical guarantees and are applicable to, e.g., social networks and biological networks.

My other main research agenda uses machine learning to design new methods in computational biology. One project develops a computational framework to find [combinatorial markers](https://www.embopress.org/doi/full/10.15252/msb.20199005) for cell populations identified with single-cell RNA-seq data. In another work, I conceived a [drug repurposing pipeline](https://www.nature.com/articles/s41467-021-21056-z) to identify candidate drugs for repurposing against SARS-CoV-2. In my current projects, I leverage network methods to characterize the relationship between protein interactions on the cell membrane and gene interactions in the nucleus and I also use Bayesian optimization and causality to better design _in vitro_ cell reprogramming experiments.

In a new avenue of research, I leverage tools from probability to better characterize the optimality of stable marriages under correlated preferences, which has implications, e.g., in the students/schools matching problem and the hospitals/residents matching problem.
<nbsp>

{% include base_path %}

{% assign ordered_pages = site.research | sort:"order_number" %}

{% for post in ordered_pages %}
  {% include archive-single.html type="grid" %}
{% endfor %}
