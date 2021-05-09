---
layout: default
title: Identifying the Source
nav_order: 6
---

# Identifying the Source

We already know the Broad St. pump was the source of the outbreak, but lets explore a couple analysis techniques we could use to identify the source of the outbreak.

## Measures of Central Tendency

There are numerous ways to analyze the spatial distribution of a dataset.  The (Mean Center)[https://pro.arcgis.com/en/pro-app/latest/tool-reference/spatial-statistics/mean-center.htm] and (Directional Distribution)[https://pro.arcgis.com/en/pro-app/latest/tool-reference/spatial-statistics/directional-distribution.htm] are two of the simplest measures.  Mean center gives you a single point around which the directional distribution is an ellipse that shows you directional trends in the data.
* They can be weighted (eg. by the number of deaths per address).
* These measures roughly identify the Broad St. Pump as the source of the outbreak, as shown in the figure below.
  * However, they are rudimentary metrics at best.  They could be used to identify multiple point sources for example.

<div style="overflow: hidden;
  padding-top: 56.25%;
  position: relative">
  <iframe src="Distribution.png" title="Processes" scrolling="no" frameborder="0"
    style="border: 0;
   height: 100%;
   left: 0;
   position: absolute;
   top: 0;
   width: 100%;">
   <p>Your browser does not support iframes.</p>
 </iframe>
</div>
<a href="Distribution.png" target="_blank">View Image in New Tab</a>


A more advanced method is [Kernel Density](https://pro.arcgis.com/en/pro-app/latest/tool-reference/spatial-analyst/kernel-density.htm), which gives you a magnitude (eg. number of deaths) per unit area (hectare).
* 


## Save your project.

Click Save in the top left of the Arc Pro window.
