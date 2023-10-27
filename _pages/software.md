---
title: "Software"
layout: gridlay
sitemap: false
permalink: /software/
---

# Software - Open Source 

<div class="rowl1">
<div class="row align-items-end">
<div class="col-md-12 col-sm-12">
<h3>GPS 2 GTFS

<a href="https://github.com/aaivu/gps2gtfs" target="_blank"><button class="btn btn-info btn-sm">GIT</button></a>
<a href="https://pypi.org/project/gps2gtfs/0.1.0/" target="_blank"><button class="btn btn-danger btn-sm">PyPI</button></a> </h3>

<h4>
*Transforming Bus GPS data to GTFS format*
</h4>
<h5>
<b>Authors:</b>
<i>Uthayasanker T., Shiveswarran R.</i></h5>
<h5>
<b>Contributors:</b>
<i>Gopinath S., Kesavi A., Kajanan S.</i></h5>


<div style="text-align:justify">

The "gps2gtfs" Python package provides a streamlined solution for preprocessing GPS (Global Positioning System) raw data and converting it into GTFS (General Transit Feed Specification) data format. Leveraging the power of DataFrame and GeoDataFrame with parallelization, this package offers efficient methods to extract essential trip details from raw GPS data. These details encompass trip sequences, stop information, arrival time to stops, departure time from stops, dwell time at stops, travel durations, running times between stops, and the seamless transformation into GTFS data structure. Currently, "gps2gtfs" handles static (schedule) trip data at heterogeneous traffic condition, with the potential for future expansion to accommodate dynamic real-time trip data. Furthermore, in the future, a visualization package can be seamlessly integrated with existing packages
The "gps2gtfs" framework is developed using Python 3, with a thoughtfully designed package structure that ensures minimal interdependence among the main packages. The core components encompass distinct packages, each serving a specific purpose: data_field, load_data, preprocessing, trip, stop, reporting, pipeline, and utility. Users are expected to provide input for a single route, and the system facilitates the inclusion of multiple routes into the pipeline through user-driven iteration.

The package is structured into eight(8) primary packages:

</div>

<div style="text-align:left">


- `data_field`: his package is responsible for managing column names for user input and a predefined set of output columns. The fields provided by the user should be a superset of the defined fields within this package.
- `load_data`: This package handles the loading of necessary data into the pipeline.
- `preprocessing`: The preprocessing package is designed to clean the data loaded from the previous step.
- `trip`: The trip package focuses on extracting trips and generating associated features.
- `stop`: Within the stop package, the identification of stops and the creation of related features take place.
- `reporting`: This package is responsible for generating outputs containing the extracted information
- `pipeline`:This package contains functionality to execute the trip extraction pipeline and the trip & stop extraction pipeline.
- `utility`: The utility module provides support for various utility functions, including input/output operations, data conversions, and logging.


</div>
</div>
</div>
</div>