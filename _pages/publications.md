---
layout: single
title: "Publications"
excerpt: "Journal articles, manuscripts under revision, and preprints by Zhiyu Xu."
permalink: /publications/
author_profile: true
redirect_from:
  - /research/
---

My work spans latent-variable models, probabilistic machine learning, and psychometrics, with applications to educational assessment and large language model evaluation.

You can also find my work on [Google Scholar]({{ site.author.googlescholar }}).

{% assign papers = site.publications | sort: 'order' %}

## Journal articles

{% for paper in papers %}
{% if paper.publication_group == 'journal' %}
{% include publication-entry.html paper=paper %}
{% endif %}
{% endfor %}

## Manuscripts under revision

{% for paper in papers %}
{% if paper.publication_group == 'revision' %}
{% include publication-entry.html paper=paper %}
{% endif %}
{% endfor %}

## Preprints

{% for paper in papers %}
{% if paper.publication_group == 'preprint' %}
{% include publication-entry.html paper=paper %}
{% endif %}
{% endfor %}
