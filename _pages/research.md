---
title: "Research"
layout: gridlay
sitemap: false
permalink: /research/
---

# Research

<div class="rowl1">
  <img src="{{ site.url }}{{ site.baseurl }}/images/respic/bat.jpg" class="img-responsive" width="20%" style="float: left; border-radius:10px" />
  <h4>Bus Travel Time Prediction using Multi-Model Ensemble Approach</h4>
An accurate and reliable arrival time prediction of buses to the next bus stops is a valuable tool for both passengers and operators. Existing studies have some limitations in bus travel time prediction. They focus little on three aspects such as heterogeneous traffic flow conditions, dwell time prediction and interpretation of explanatory variables. Consequently, we break down the prediction problem into sub-models for running time and dwell time prediction and incorporate a feature engineering framework that generates features related to the running bus, the prediction day, and immediate and historical time variations to capture heterogeneous traffic conditions. We propose a multi- model stacked generalisation ensemble model by leveraging the advantages of best-performing models in homogeneous conditions such as Extreme Gradient Boosting (XGBoost) and convolutional long short-term memory (ConvLSTM) models. It outperformed the state-of-the-art models by 11% in mean absolute error (MAE) on average. It can predict extreme conditions in bus journeys more accurately. When interpreting the feature importance, we found insights like driver behaviour and preceding travel time influence the prediction model, which paves the way for strategic management by authorities."
  <ul style="overflow: hidden">
  </ul>
</div>
 

<div class="rowl1">
  <img src="{{ site.url }}{{ site.baseurl }}/images/respic/gps.jpg" class="img-responsive" width="20%" style="float: left; border-radius:10px" />
  <h4>Extracting potential Travel time information from raw GPS data of buses</h4>
The widespread use of location-enabled devices on public transportation vehicles produces a huge amount of geospatial data. The primary objective of this research study is to build a solution framework that can process a large amount of geospatial data obtained from GPS (Global Positioning System) receivers fixed on different buses on different routes, preprocess, clean, and transform that data for analysis. There are various challenges associated with the processing of GPS data, like discontinuities, non-uniformities, poor network coverage, and human errors. This study proposes two novel, simple algorithms to extract bus trip and bus stop sequences, from the crude raw data, incorporating those challenges. Moreover, the dwell times at the bus stops are estimated solely using this GPS data in three different possible scenarios in the data filtering process. When considering the previous related studies in this area, the proposed approaches are applied to GPS data obtained at a medium sample rate (for example, 15 seconds) for heterogeneous traffic conditions, and also with a unique dwell time estimation process. In addition, statistical methods are implemented to analyse a variety of novel public transit-system performance metrics, such as (i) excess journey time (EJT); (ii) excess dwelling time (EDT); (ii) excess running time (ERT); and (iv) segment idle time ratio (SITR), at different time horizons, where these metrics are developed in the absence of schedule data. These metrics facilitate the transport authorities in real-time bus monitoring, evaluating their performance, and identifying inappropriate driving behaviours. A detailed explanation is provided through a case study of two main routes in the Kandy district of Sri Lanka."

  <ul style="overflow: hidden">
  </ul>
</div>

