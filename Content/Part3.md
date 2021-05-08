---
layout: default
title: Foundations of Epidemiology
nav_order: 4
---

# Foundations of Epidemiology: Identifying Sources of Cholera Outbreaks

Dr. John Snow (1813 – 1858) is credited as one of the founders of modern Epidemiology (the study and analysis of the distribution of diseases).  He was a physician practicing in London where cholera outbreaks were a frequent occurrence due to poor sanitation practices.  Dr. Snow was a skeptic of the miasma theory and a proponent of germ theory.  In 1849 Dr. Snow proposed cholera that it was spread by contaminated water, after comparing cholera rates between London districts supplied by different water companies.  Five years later, during an outbreak in London's SoHo neighborhood in 1854, Dr. Snow was able to identify the point source of an the outbreak using a hand-sketched map.  He recorded each case of cholera in the area using a dash, and recorded each water pump with a circled dot, creating what today would be called a ‘dot map.’ By recording clusters of disease, and conducting interviews, Snow was able to trace most cases of the outbreak to a single water pump, located on Broad st.

<div style="overflow: hidden;
  padding-top: 56.25%;
  position: relative">
  <iframe src="Snow_Map.jpg" title="Processes" scrolling="no" frameborder="0"
    style="border: 0;
   height: 100%;
   left: 0;
   position: absolute;
   top: 0;
   width: 100%;">
   <p>Your browser does not support iframes.</p>
 </iframe>
</div>
<a href="Snow_Map.jpg" target="_blank">View Image in New Tab</a>


### Applying Modern Methods to the 1854 Cholera Outbreak in London 

We're going to work with Dr. Snow's original data and replicate the study using modern GIS methods.  In order to get the map into a GIS, it has to be scanned and then [georeferenced](https://pro.arcgis.com/en/pro-app/latest/help/data/imagery/overview-of-georeferencing.htm).  To georeference a map like this, points on the scanned map (eg. intersections) can be matched up to an existing map.  With enough matching points, an accurate transformation can be calculated and the paper map can be projected over base map.  Watch this video for a quick overview of georeferencing.

Once the map has been scanned and georeferenced, we can extract information from it.  On Dr. Snow’s map, the key pieces of information are the cholera deaths and water pumps.  To get this information into the GIS, the points manually identify identified and entered.  This process is known as digitizing, and was explained in the [Create points on a map](https://pro.arcgis.com/en/pro-app/latest/get-started/create-points-on-a-map.htm) video.  The deaths layer has already been digitized, you can add it to the map by following these steps and referencing the video:
* Opening the catalog pane and navigating to your Lab1_Project.
* Find the Deaths feature class in the Source Points feature dataset.  Click and drag the deaths feature class onto the map area.
* Right click on the Deaths layer in the table of contents and click zoom to layer.
* Once zoomed in, right click again and open the attribute table to explore the data a bit.
  * You can double click count to sort in ascending/descending order.
  * Click a row to select a specific feature (eg. identify location with most deaths)

<div style="overflow: hidden;
  padding-top: 56.25%;
  position: relative">
  <iframe src="AddData.mp4" title="Processes" scrolling="no" frameborder="0"
    style="border: 0;
   height: 100%;
   left: 0;
   position: absolute;
   top: 0;
   width: 100%;">
   <p>Your browser does not support iframes.</p>
 </iframe>
</div>
<a href="AddData.mp4" target="_blank">View Image in New Tab</a>

## **Question 8)**
How many cholera deaths were recorded in this outbreak?  Right click "COUNT" in the attribute table and choose "Statistics" as shown below.  A chart window and a properties pane will open.  Use the statistics in the properties pane to answer the question.

<div style="overflow: hidden;
  padding-top: 56.25%;
  position: relative">
  <iframe src="Statistics.png" title="Processes" scrolling="no" frameborder="0"
    style="border: 0;
   height: 100%;
   left: 0;
   position: absolute;
   top: 0;
   width: 100%;">
   <p>Your browser does not support iframes.</p>
 </iframe>
</div>
<a href="Statistics.png" target="_blank">View Image in New Tab</a>


The map is already georeferenced for you and the point data has already been extracted.

• In the top left, under the insert tab, click New Map
o As in Part 2, rename the new map Part 3
• Under the View tab, click Catalog Pane.  This will dock the Catalog Pane on the right side of your window, showing a file tree.  Your window should now look something like the image below.
• You now know two ways to access the Catalog.  The Catalog window and the Catalog pane.  The Catalog window shows more detailed information, allowing you to inspect the metadata.  While the Catalog Pane just shows the file tree and is a quick way to navigate folders and add data.
• In the Catalog Pane, under Folders/lab2_data expand the CholeraOutbreak_1854.gdb
o Click on Snow_cholera_map and drag it onto your Part 3 map area.  The scanned map from Dr. Snow’s original work should load, and the map area will be centered on the Soho neighborhood of London. Your map should now look like show below.  Toggle the Snow_cholera_map on and off to see how things in Soho look now compared to 1854.

<div style="overflow: hidden;
  padding-top: 56.25%;
  position: relative">
  <iframe src="New_Project.png" title="Processes" scrolling="no" frameborder="0"
    style="border: 0;
   height: 100%;
   left: 0;
   position: absolute;
   top: 0;
   width: 100%;">
   <p>Your browser does not support iframes.</p>
 </iframe>
</div>
<a href="New_Project.png" target="_blank">View Image in New Tab</a>

