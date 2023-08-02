---
title: "Service"
layout: gridlay
sitemap: false
permalink: /service/
---


{% if site.data.teaching %}
# Teaching

{% for publi in site.data.teaching %}
* {{ publi.name }}
{% endfor %}
{% endif %}



{% if site.data.academic_service %}
# International Conference Reviewing

{% for publi in site.data.academic_service %}
* {{ publi.name }}
{% endfor %}
{% endif %}

