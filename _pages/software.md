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
<img src="{{site.url}}{{site.baseurl}}/images/Software/pydeepp2sa.jpg" style="width:100px; min-width:10%; max-width:100%; margin-left:20px; margin-right:0px; margin-bottom:0px; margin-top:15px;" align="right"/>
<h3>pyDeepP2SA (In development)

<a href="https://github.com/BrinthanK/pyDeepP2SA" target="_blank"><button class="btn btn-info btn-sm">GIT</button></a>
<a href="https://pypi.org/project/pyDeepP2SA/" target="_blank"><button class="btn btn-danger btn-sm">PyPI</button></a> </h3>

<h4>
*Advanced Particle Size and Shape Analysis with Python*
</h4>
<h5>
<b>Author:</b>
<i>Brinthan K.</i></h5>


<div style="text-align:justify">

An advanced particle size and shape analysis (P2SA) package powered by the cutting-edge Segment Anything Model (SAM) developed by Facebook Inc. This package provides highly accurate and robust object segmentation, revolutionising the field of P2SA by offering a zero-generalisation segmentation technique. With minimal manual intervention, pyDeepP2SA delivers exceptional results and simplifies the entire analysis workflow.  

pyDeepP2SA provides several useful functions for particle size and shape analysis:
</div>

<div style="text-align:left">


- `generate_masks(image, sam_checkpoint, points_per_side=32, pred_iou_thresh=0.95, stability_score_thresh=0.9, crop_n_layers=1, crop_n_points_downscale_factor=2, min_mask_region_area=100)`: Generates masks for an input image using a SAM checkpoint.
- `visualise_masks(image, masks)`: Visualises the segmented image with the generated masks.
- `save_masks_to_csv(masks, csv_directory, pixel_to_micron)`: Saves the generated masks to a CSV file along with calculated region properties.
- `plot_diameters(image, masks, diameter_threshold, circularity_threshold, pixel_to_micron)`: Plots the original image with bounding boxes around masks that meet specified diameter and circularity thresholds.
- `ind_mask(masks, diameter_threshold, circularity_threshold, pixel_to_micron, image)`: Filters masks based on diameter and circularity thresholds and plots the filtered masks along with their region properties.
- `stat_sum(diameter_threshold, circularity_threshold, csv_directory)`: Reads the CSV file with region properties and returns a summary of properties for masks that meet specified diameter and circularity thresholds.
- `plot_boxplots(diameter_threshold, circularity_threshold, csv_directory)`: Reads the CSV file and plots boxplots for the area, perimeter, diameter, and circularity of masks that meet specified diameter and circularity thresholds.
- `plot_psd(diameter_threshold, circularity_threshold, csv_directory)`: Reads the CSV file and plots the particle size distribution (PSD) using a histogram and cumulative frequency curve.
- `plot_cir(diameter_threshold, circularity_threshold, csv_directory)`: Reads the CSV file and plots the circularity distribution using a histogram.

</div>
</div>
</div>
</div>

<div class="rowl1">
<div class="row align-items-end">
<div class="col-md-12 col-sm-12">
<img src="{{site.url}}{{site.baseurl}}/images/Software/pychemeng.jpg" style="width:100px; min-width:10%; max-width:100%; margin-left:20px; margin-right:0px; margin-bottom:0px; margin-top:15px;" align="right"/>
<h3>pyChemEng
<a href="https://github.com/Ashane-F/pyChemEng" target="_blank"><button class="btn btn-info btn-sm">GIT</button></a>
<a href="https://pypi.org/project/pyChemEng/" target="_blank"><button class="btn btn-danger btn-sm">PyPI</button></a> </h3>

<h4>
*Adsorption Isotherm and Kinetic Models with Python Package* </h4>
<h5>
<b>Authors:</b>
<i>Brinthan K. and Dr Ashane Fernando</i></h5>


<div style="text-align:justify">

pyChemEng is a Python package for understanding and representing multiple adsorption and kinetic models in the chemical thermodynamics spectrum. This project is an initiative considering research scientists for the unequivocal representation of the models with all the useful information.

Currently, our package supports the following adsorption isotherm models:

- Langmuir
- Freundlich
- Toth
- Sips
- Temkin
- Dubinin

The adsorption kinetic models currently supported by our package are:

- Pseudo First Order (PFO)
- Pseudo Second Order (PSO)
- Elovich
- Sips
- Temkin
- Dubinin

</div>
</div>
</div>
</div>