---
layout: single
title: "Publications"
permalink: /publications/
---

## Journal articles
{% assign pubs = site.data.publications | where: "type", "publication" | sort: "year" | reverse %}
{% for p in pubs %}
- **{{ p.title }}** ({{ p.year }}). {{ p.authors }}. _{{ p.venue }}_.  
  {% if p.doi %}[DOI]({{ p.doi }}){% endif %}
  {% if p.pdf %} · [PDF]({{ p.pdf }}){% endif %}
  {% if p.code %} · [Code]({{ p.code }}){% endif %}
  {% if p.slides %} · [Slides]({{ p.slides }}){% endif %}
  {% if p.video %} · [Video]({{ p.video }}){% endif %}
{% endfor %}

---

## Preprints
{% assign preprints = site.data.publications | where: "type", "preprint" | sort: "date" | reverse %}
{% for p in preprints %}
- **{{ p.title }}** ({{ p.year }}). {{ p.authors }}. _{{ p.venue }}_.  
  {% if p.doi %}[DOI]({{ p.doi }}){% endif %}
  {% if p.pdf %} · [PDF]({{ p.pdf }}){% endif %}
  {% if p.code %} · [Code]({{ p.code }}){% endif %}
{% endfor %}

## Software
{% assign software = site.data.publications | where: "type", "software" | sort: "date" | reverse %}
{% for p in preprints %}
- **{{ p.title }}** ({{ p.year }}). {{ p.authors }}. _{{ p.venue }}_.  
  {% if p.doi %}[DOI]({{ p.doi }}){% endif %}
  {% if p.pdf %} · [PDF]({{ p.pdf }}){% endif %}
  {% if p.code %} · [Code]({{ p.code }}){% endif %}
{% endfor %}