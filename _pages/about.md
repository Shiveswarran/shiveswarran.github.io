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

I am a research assistant at the <a href="http://datasearch.uom.lk/2/index.php"> DataSEARCH research center</a>, Department of Computer Science and Engineering (CSE), University of Moratuwa. I have completed my Master's research degree at the Dept of CSE in the theme of intelligent transportation systems with a focus on improving public transportation service in Sri Lanka. My research encompasses predictive modelling of bus arrival times through advanced machine learning paradigms like <span style="color:#61B886;"> spatio-temporal forecasting, meta-learning, ensemble learning and explainable AI </span>. 

At present, my primary research emphasis lies on spatio-temporal data (e.g. GPS) processing and <span style="color:#E5E3C4;"> mathematical modelling of trajectories </span> of bus trips. I am actively involved in exploring various modelling methods and improving the prediction accuracy and hence, reliability. Through my work, I endeavour to contribute to the enhancement of public transportation systems in my country. By utilising advanced machine learning techniques and computational methods, I strive to unearth new insights and potential applications of advanced machine learning techniques in spatio-temporal data, ultimately fostering a more reliable public transits

<br/>

</div>

<div class="rowl1">

## Areas of Research Interests 

- Intelligent Transportation Systems
- Advanced Machine Learning
- Time Series Forecasting 
- Spatial Data Science
- Explainable AI
- Connected & Autonomous vehicles
- Sustainability

<br/>

</div>



<div class="rowl1">

## Latest Publications (2023 only)

{% for publi in site.data.publist %}
{% if publi.year == 2023 %}

{% assign bibtest = false %}
{% if publi.url %}
{% assign bibfile = "/papers/" | append:  publi.url  | append: ".txt" %}
{% for file in site.static_files %}
  {% if file.path contains bibfile %}
   {% assign bibtest = true %}
  {% endif %}
{% endfor %}
{% endif %}

<div class="well-sm">
<ul class="flex-container">
<li class="flex-item1">
  {% if publi.image %}
   <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="100%" style="float: left" />
  {% endif %}
</li>
<li class="flex-item2">
  <strong> {{ publi.title }}</strong><br/>
  <em>{{ publi.authors }} </em><br/>
  {{ publi.display }}<br/>
  {% if publi.url %}<a href="{{ site.url }}{{ site.baseurl }}/papers/{{ publi.url }}.pdf" target="_blank"><button class="btn-pdf">PDF</button></a>{% endif %}
  {% if publi.doi %}<a href="http://dx.doi.org/{{ publi.doi }}" target="_blank"><button class="btn-doi">DOI</button></a> {% endif %}
  {% if publi.arxiv %}<a href="https://arxiv.org/abs/{{ publi.arxiv }}" target="_blank"><button class="btn-arxiv">ARXIV</button></a> {% endif %}
  {% if bibtest == true %} <a data-toggle="collapse" href="#{{publi.url}}2"  class="btn-bib" style="text-decoration:none; color:#ebebeb; hover:#ebebeb;" role="button" aria-expanded="false" aria-controls="{{publi.url}}2">BIB</a> {% endif %}
  {% if publi.abstract %} <a data-toggle="collapse" href="#{{publi.url}}"  class="btn-abstract" style="text-decoration:none; color:#ebebeb; hover:#ebebeb;" role="button" aria-expanded="false" aria-controls="{{publi.url}}">ABSTRACT</a> {% endif %}

{% if publi.abstract %}
<div class="collapse" id="{{publi.url}}"><div class="well-abstract">
 {{publi.abstract}}
</div></div>
{% endif %}

{% if bibtest == true %}
<div class="collapse" id="{{publi.url}}2"><div class="well-bib">
 <iframe src='{{site.url}}{{site.baseurl}}/papers/{{publi.url}}.txt' scrolling='yes' width="100%" height="210" frameborder='0'></iframe>
</div></div>
{% endif %}

</li>
</ul>
</div>
{% endif %}
{% endfor %}

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

For additional details and materials related to presentations, kindly click <a href="https://shiveswarran.github.io/Presentations/">here</a>.

<br/>
</div>

<div class="rowl1">

## Key Research Skills

- Advanced Machine Learning techniques.
- Time series forecasting and predictive modelling.
- Spatial - Temporal Data Science and analytics
- Intelligent transportation systems 
- Advanced feature engineering and Interpretation of black box machine learning models
- Simulation design, performance analysis, and optimisation for developing efficient and accurate computational models and simulations.
- Statistical learning methods for analysing complex data-sets and drawing meaningful conclusions.
- Strong programming skills in Python and R for implementing algorithms, data manipulation, and statistical analysis for scientific computing.
- Proficiency in LaTeX and markdown markup languages for creating professional and well-formatted research documents and reports.

<br/>
</div>


<div class="rowl1">

{% if site.data.reviewer %}
## Academic Services

#### International Conference Reviewing

{% for service in site.data.reviewer %}
* {{ service.name }}
{% endfor %}


#### Workshops

{% for service in site.data.workshops %}
* {{ service.name }}
{% endfor %}

#### Mentorship

{% for service in site.data.mentorship %}
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



