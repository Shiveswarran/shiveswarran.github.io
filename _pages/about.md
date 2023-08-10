---
title: "About"
layout: gridlay
sitemap: false
permalink: /about/
---

## About 


{% for member in site.data.pi %}

<div class="row">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="30%" style="float: left" />
  <h3>{{ member.name }}</h3>
  <i style="font-size:20px">{{ member.info }}</i><br>

  {% if member.website %}<a href="{{ member.website }}" target="_blank"><i class="fa fa-home fa-3x"></i></a> {% endif %}
  {% if member.email %}<a href="mailto:{{ member.email }}" target="_blank"><i class="fa fa-envelope-square fa-3x"></i></a> {% endif %}
  {% if member.scholar %} <a href="{{ member.scholar }}" target="_blank"><i class="ai ai-google-scholar-square ai-3x"></i></a> {% endif %}
  {% if member.cv %} <a href="{{ member.cv }}" target="_blank"><i class="ai ai-cv-square ai-3x"></i></a> {% endif %}
  {% if member.github %} <a href="{{ member.github }}" target="_blank"><i class="fa fa-github-square fa-3x"></i></a> {% endif %}
  {% if member.researchgate %} <a href="{{ member.researchgate }}" target="_blank"><i class="ai ai-researchgate-square ai-3x"></i></a> {% endif %}
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  {% if member.number_educ == 6 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  <li> {{ member.education6 }} </li>
  {% endif %}

  {% if member.number_educ == 7 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  <li> {{ member.education6 }} </li>
  <li> {{ member.education7 }} </li>
  {% endif %}

  </ul>
</div>


{% endfor %}

<div class="row" style="text-align:justify">


<div class="rowl1">

## Short Biography 

I am a postgraduate student at the University of Moratuwa, pursuing a Master's research project in the exploration and characterisation of coal fly ash, a waste material, with a focus on advancing material usage. My research encompasses mineral processing through separation technology, material synthesis and characterisation, machine learning, and digital image processing. At present, my primary research emphasis lies in <span style="color:#E5E3C4;">computational X-ray microanalysis</span> and its applications for materials at the nano- and micron-scale. I am actively involved in <span style="color:#E5E3C4;">simulations and computational decision-making processes</span> aimed at characterising nano and micron materials derived from coal fly ash. Through my work, I endeavour to contribute to the scientific understanding of coal fly ash as a valuable resource for sustainable material development. By utilising advanced analytical techniques and computational methods, I strive to unearth new insights and potential applications for this waste material, ultimately fostering a more environmentally conscious approach.

<br/>

</div>



<div class="rowl1">

## Publications


For a comprehensive list of publications, kindly click <a href="https://brinthank.github.io/publications/">here</a>.

<br/>

</div>


<div class="rowl1">

## Presentations

{% if site.data.conference_talks_oral %}
#### Oral Presentations

{% for publi in site.data.conference_talks_oral %}
* <strong>{{ publi.title }}</strong> <br/> <i>{{ publi.authors }}</i>, {{ publi.conf }} ({{ publi.year }})
{% endfor %}
{% endif %}

{% if site.data.conference_talks_poster %}
#### Poster Presentations

{% for publi in site.data.conference_talks_poster %}
* <strong>{{ publi.title }}</strong> <br/> <i>{{ publi.authors }}</i>, {{ publi.conf }} ({{ publi.year }})
{% endfor %}
{% endif %}

For additional details and materials related to presentations, kindly click <a href="https://brinthank.github.io/Presentations/">here</a>.

<br/>
</div>

<div class="rowl1">

## Key Research Skills

- Advanced computer vision techniques.
- Machine learning data analysis, pattern recognition, and predictive modelling.
- Physics informed machine learning.
- Digital image processing for advanced microscopy analysis.
- Material characterisation using advanced imaging and spectroscopy techniques for studying material properties and composition.
- Computational X-ray micro-analysis methods for analysing and interpreting X-ray data to extract information.
- Simulation design, performance analysis, and optimisation for developing efficient and accurate computational models and simulations.
- Statistical learning methods for analysing complex data-sets and drawing meaningful conclusions.
- Strong programming skills in Python and R for implementing algorithms, data manipulation, and statistical analysis for scientific computing.
- Proficiency in LaTeX and markdown markup languages for creating professional and well-formatted research documents and reports.

<br/>
</div>


<div class="rowl1">

{% if site.data.academic_service %}
## International Conference Reviewing

{% for service in site.data.academic_service %}
* {{ service.name }}
{% endfor %}

{% endif %}

<br/>
</div>

<div class="rowl1">

{% if site.data.awards %}
## Grants and Awards

{% for award in site.data.awards %}
* {{ award.name }}
{% endfor %}

{% endif %}

<br/>
</div>






</div>

