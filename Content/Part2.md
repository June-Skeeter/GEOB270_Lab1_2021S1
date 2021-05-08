---
layout: default
title: Part 2
nav_order: 3
---

# Miasma vs. Germ Theory

Early forms of [germ theory](https://en.wikipedia.org/wiki/Germ_theory_of_disease), the concept that disease transmission is driven by pathogens, emerged around the world more than 2000 years ago.  By the middle ages, Islamic physicians had formally proposed the basics of germ theory.  For example, writing about an outbreak of the bubonic plague in [1362](https://en.wikipedia.org/wiki/Ibn_al-Khatib#On_the_Plague), Ibn al-Khatib astutely pointed out:

* *"The existence of contagion is established by experience [and] by trustworthy reports on transmission by garments, vessels, ear-rings; by the spread of it by persons from one house, by infection of a healthy sea-port by an arrival from an infected land [and] by the immunity of isolated individuals."*  

Regardless this knowledge European scientists physicians clung to the [miasma theory](https://en.wikipedia.org/wiki/Miasma_theory) which attributed diseases such as cholera to “bad air” for many centuries.  In the face of mounting evidence many doctors and public officials stubbornly refused to acknowledge that basic hygiene and sanitation could save lives.  Here is one striking historical example:

* The Vienna Maternity Hospital had two maternity clinics with vastly different maternal mortality rates.  Between 1840 and 1846, the maternal mortality rate was 10% at the clinic run by physicians and medical students but only 4% at the clinic run by midwives.  The doctors/students started each day with postmortem examinations of deaths from the previous day, then proceeded to the maternity ward without washing their hands.  By contrast, the midwives didn't do postmortems.  In 1847, the newly appointed chief resident Ignaz Semmelweis suspected contagions from the cadavers were to blame.  Semmelweis mandated hand washing and sanitizing instruments with a chlorine solution entering both clinics.  By 1848, the maternal mortality rate in both clinics fell to 1.3% (Loudon, 2013).
* Despite the overwhelming evidence in favor of sanitizing, Semmelweis' methods were rejected by the medical community in Europe because they were in conflict with the Miasma theory.  Antisepsis was not routinely incorporated into obstetric practice until the 1880s.

# The foundations of Epidemiology: Identifying the source of cholera outbreaks

Dr. John Snow (1813 – 1858), a skeptic of the miasma theory and a proponent of germ theory is credited as one of the founders of modern Epidemiology (the study and analysis of the distribution of diseases).  He was a physician practicing in London where cholera outbreaks were a frequent occurrence due to poor sanitation practices.  Dr. Snow studied Cholera and in 1849 proposed that it was spread by contaminated water, comparing Cholera rates between districts supplied by different water companies with different sources and sanitation practices.  During an outbreak in London's SoHo neighborhood in 1854, by talking with local residents and searching through official case records, Snow was able to identify a point source for the outbreak using a hand-sketched map. he recorded each case of cholera in the area using a dash, and recorded each water pump with a circled dot, creating what today would be called a ‘dot map.’ By recording clusters of disease, and conducting interviews, Snow was able to trace most cases of the outbreak to a single water pump, located on Broad st.

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

Once the map has been scanned and georeferenced, we can extract information from it.  On Dr. Snow’s map, the key pieces of information are the cholera deaths and water pumps.  The process of creating a new layer from an existing map is called [digitizing]()

Adding and Editing the Data

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
