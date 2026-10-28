---
layout: single
title: "Research"
excerpt: "Research on latent-variable models, probabilistic machine learning, and psychometrics."
permalink: /research/
author_profile: true
---

My research interests include latent-variable models, probabilistic machine learning, and psychometrics, with applications to educational assessment and large language model evaluation.

See [Publications]({{ '/publications/' | relative_url }}) for the publication list or [Google Scholar]({{ site.author.googlescholar }}) for my scholar profile. The contributions below describe my individual work on each project.

{% assign research = site.publications | sort: 'order' %}
{% for paper in research %}
## [{{ paper.title }}]({{ paper.url | relative_url }})

{{ paper.authors }}{% if paper.author_note %} ({{ paper.author_note }}){% endif %}. {{ paper.year }}.

*{{ paper.status }}.*

{% include research-links.html paper=paper %}

{{ paper.content | markdownify }}
{% endfor %}
