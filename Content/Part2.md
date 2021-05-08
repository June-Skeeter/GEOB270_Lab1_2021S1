---
layout: default
title: Part 2
nav_order: 3
---

# Miasma Theory vs. Germ Theory

Early forms of [germ theory](https://en.wikipedia.org/wiki/Germ_theory_of_disease), the concept that disease transmission is driven by pathogens, emerged around the world more than 2000 years ago.  By the middle ages, Islamic physicians had formally proposed the basics of germ theory.  For example, writing about an outbreak of the bubonic plague in [1362](https://en.wikipedia.org/wiki/Ibn_al-Khatib#On_the_Plague), Ibn al-Khatib astutely pointed out:

* *"The existence of contagion is established by experience [and] by trustworthy reports on transmission by garments, vessels, ear-rings; by the spread of it by persons from one house, by infection of a healthy sea-port by an arrival from an infected land [and] by the immunity of isolated individuals."*  

Regardless this knowledge European physicians clung to the [miasma theory](https://en.wikipedia.org/wiki/Miasma_theory) which attributed diseases such as cholera to “bad air” for many centuries.  In the face of mounting evidence many doctors and public officials stubbornly refused to acknowledge that basic hygiene and sanitation could save lives.  Here is one striking historical example:

* The Vienna Maternity Hospital had two maternity clinics with vastly different maternal mortality rates.  Between 1840 and 1846, the maternal mortality rate was 10% at the clinic run by physicians and medical students but only 4% at the clinic run by midwives.  The doctors/students started each day with postmortem examinations, then proceeded to the maternity ward without washing their hands.  By contrast, the midwives didn't do postmortem exams.  In 1847, the new chief resident Ignaz Semmelweis suspected contagions from the cadavers were to blame.  Semmelweis mandated hand washing and sanitizing instruments with a chlorine solution for both clinics.  By 1848, the maternal mortality rate in both clinics fell to 1.3% (Loudon, 2013).
* Despite the overwhelming evidence in favor of sanitizing, Semmelweis' methods were rejected by the medical community in Europe because they were in conflict with the Miasma theory.  Antisepsis was not routinely incorporated into obstetric practice until the 1880s.

### Question 6)
What does this above example tell you about ???

# Identifying the Source of Cholera Outbreaks: Foundations of Epidemiology

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

### Question 7)
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

•	In the top left, under the insert tab, click New Map
o	As in Part 2, rename the new map Part 3
•	Under the View tab, click Catalog Pane.  This will dock the Catalog Pane on the right side of your window, showing a file tree.  Your window should now look something like the image below.
•	You now know two ways to access the Catalog.  The Catalog window and the Catalog pane.  The Catalog window shows more detailed information, allowing you to inspect the metadata.  While the Catalog Pane just shows the file tree and is a quick way to navigate folders and add data.
•	In the Catalog Pane, under Folders/lab2_data expand the CholeraOutbreak_1854.gdb
o	Click on Snow_cholera_map and drag it onto your Part 3 map area.  The scanned map from Dr. Snow’s original work should load, and the map area will be centered on the Soho neighborhood of London. Your map should now look like show below.  Toggle the Snow_cholera_map on and off to see how things in Soho look now compared to 1854.

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




# References

Loudon, I. (2013). Ignaz Phillip Semmelweis’ studies of death in childbirth. Journal of the Royal Society of Medicine, 106(11), 461–463. https://doi.org/10.1177/0141076813507844
