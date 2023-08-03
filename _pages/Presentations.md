---
title: "Presentations"
layout: gridlay
sitemap: false
permalink: /Presentations/
---

# Presentations

{% if site.data.conference_talks_oral %}
## Oral Presentations

{% for publi in site.data.conference_talks_oral %}
* <strong>{{ publi.title }}</strong> <br/> <i>{{ publi.authors }}</i>, {{ publi.conf }} ({{ publi.year }})
{% endfor %}
{% endif %}

{% if site.data.conference_talks_poster %}
## Poster Presentations

{% for publi in site.data.conference_talks_poster %}
* <strong>{{ publi.title }}</strong> <br/> <i>{{ publi.authors }}</i>, {{ publi.conf }} ({{ publi.year }})
{% endfor %}
{% endif %}