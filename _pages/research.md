---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
header:
  og_image: "research/ecdf.png"
---

My research falls into two main areas: developing new methods and theory in network systems, and addressing complex problems in biology using machine learning techniques on modern omics data. One strand of research in this first area develops a novel statistically optimal and computationally tractable test for detecting the presence of communities in networks in which agents can simultaneously belong to several communities. My interest in time-evolving networks also informs a current methodological project on the estimation of mixed memberships in dynamic network models. The methods I design come with strong statistical guarantees and are applicable to analyze, e.g., social networks and biological networks.

My other main research agenda uses machine learning to develop new methods in computational biology. One project develops a computational framework for the identification of combinatorial marker panels for cell populations identified with single-cell RNA-seq data. In another work, I conceived a drug repurposing pipeline to identify in silico candidate drugs for repurposing against SARS-CoV-2. In my current projects, I leverage network methods to characterize the relationship between protein interactions on the cell membrane and gene interactions in the nucleus and I also use Bayesian optimization and causality to better inform _in vitro_ cell reprogramming experiments.

In a new avenue of research, I leverage tools from probability to better characterize the optimality of stable marriages under correlated preferences, which has implications, e.g., for the students/schools matching problem and the hospitals/residents matching problem.
<nbsp>

{% include base_path %}

{% assign ordered_pages = site.research | sort:"order_number" %}

{% for post in ordered_pages %}
  {% include archive-single.html type="grid" %}
{% endfor %}
