---
title: "Home"
layout: homelay
sitemap: false
permalink: /
---

<style>
code {padding: 6px 8px; font-size: 90%;}
</style>

# Welcome!
<div class="row" style="text-align:justify">

I am a postgraduate student at the University of Moratuwa, pursuing a Master's research project in the exploration and characterisation of coal fly ash, a waste material, with a focus on advancing material usage. My research encompasses mineral processing through separation technology, material synthesis and characterisation, machine learning, and digital image processing. At present, my primary research emphasis lies in <span style="color:#1DA6DB;">computational X-ray microanalysis</span> and its applications for materials at the nano- and micron-scale. I am actively involved in <span style="color:#1DA6DB;">simulations and computational decision-making processes</span> aimed at characterising nano and micron materials derived from coal fly ash. Through my work, I endeavour to contribute to the scientific understanding of coal fly ash as a valuable resource for sustainable material development. By utilising advanced analytical techniques and computational methods, I strive to unearth new insights and potential applications for this waste material, ultimately fostering a more environmentally conscious approach.

</div>

### Active Learning for Discovering Extremes

My recent research activity at MIT centers around discovery and prediction of extreme
events by leveraging recent advancements in deep neural networks and Bayesian
statistics. Check out this quick 3 minute <a href="https://www.youtube.com/watch?v=ZYbB9TayxmQ" target="_blank">video</a> for a snapshot into my current work. Please check out our publication page form my information on this work.

<br/>

<div class="row" style="text-align:center">
<video controls autoplay muted loop width="90%" style="display:inline-block; border-radius: 25px; border:0px solid #FFF;">
  <source src="{{ site.url }}{{ site.baseurl }}/images/videos/jet_spod_resolvent.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
  Spectral Proper Orthogonal Decomposition and Resolvent Analysis of a Mach 1.5 jet. 
<br/>
Pickering et al., *Journal of Fluid Mechanics* (2020)
</div>
<br/>

### Data-Driven Turbulence Modeling

My research investigates the fundamental mechanisms that exist in complex and chaotic fluid flows by leveraging large, high-fidelity datasets to inform and validate reduced-order modeling strategies. These mechanisms are of importance as they govern engineering quantities such as noise, drag, and efficiency. Unfortunately, both high-fidelity datasets and reduced order models, alone, can only provide limited insight into these mechanisms. In much of my research, I look to pose optimization problems where our models assimilate/learn various properties of turbulence from the data to yield reduced-order models that are both predictive and general (i.e. applicable to other flows geometries and conditions). In short, this research takes a constrained-''machine learning'' approach, where the Navier-Stokes equations remain a central component of the model.


To learn from the data, turbulent flows are decomposed into their most energetic components (using Spectral Proper Orthogonal Decomposition) and then modeled via linear amplification theory of the equations of motion (Resolvent Analysis). Check out the video above on how we decompose massive datasets (numerous TB) into SPOD modes and then seek to model their theoretical equivalent with resolvent analysis.


<br/>
<div class="well-md">
<h3>Sponsors</h3>
<div style='display:block; text-align:center; margin-left:auto; margin-right:auto;'>
 {% for funder in site.data.funders %}{% if funder.url %}<a href="{{funder.url}}" target="_blank"><img src='/images/logopic/{{ funder.image }}' style='max-height: 70px; max-width: 170px;'/></a>{% else %}<img src='/images/logopic/{{ funder.image }}' class='mycenter' style='max-height: 70px; max-width: 170px;'/>{% endif %}   {% endfor %}
</div>

</div>


