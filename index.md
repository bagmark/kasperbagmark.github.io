---
layout: single
title: "Home"
---

# Kasper Bågmark

I am a PhD candidate working on deep density filtering, Bayesian inference for SDEs, stochastic neural fields, and uncertainty quantification.

- **CV:** [PDF](/assets/KasperBagmark_CV.pdf){:target="_blank"} (placeholder)
- **Google Scholar:** <https://scholar.google.com/citations?user=-oZDUnQAAAAJ>
- **GitHub:** <https://github.com/bagmark>
- **Website:** <https://bagmark.wordpress.com>

## Featured video
<!-- Example YouTube embed (replace VIDEO_ID or remove the section) -->
{% include youtube.html id="VIDEO_ID" title="Talk title here" %}

## Recent publications
{% for p in site.data.publications %}
- **{{ p.title }}**. {{ p.authors }}. _{{ p.venue }}_ ({{ p.year }}).
  {% if p.doi %}[DOI]({{ p.doi }}){% endif %}
  {% if p.pdf %} · [PDF]({{ p.pdf }}){% endif %}
  {% if p.code %} · [Code]({{ p.code }}){% endif %}
  {% if p.slides %} · [Slides]({{ p.slides }}){% endif %}
{% endfor %}

