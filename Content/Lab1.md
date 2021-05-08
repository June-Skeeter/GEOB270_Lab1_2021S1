---
layout: default
title: Lab 1 Instructions
nav_order: 2



# Setting Up & Saving Your Work

See the Lab Details page for information on how to access ArcPro using your own computer or a Geography Department computer.
* If you are using ArcPro installed on your own computer, you can manage your files however works best for you.  However, if you are working on a Geography lab computer, follow the instructions on the lab details page closely.

# Part 1: ArcGIS Pro Tutorial

To get familiar with ArcGIS Pro, you will complete an Introduction to ArcGIS Pro tutorial and watch a three other short videos.  The tutorial will give you a brief overview of the ArcGIS Pro and the videos that illustrate aspects of the software package.  If you have purchased ArcGIS Pro, you can sign in through the UBC ArcGIS online account you created. If you are using the lab computers, and don’t already have one, create a public account:
* Click "Sign In" in the top right of [this page](https://www.esri.com/training/)
* Click "Create a public account" and follow the steps

## Completing the tutorial
Go to the [Introducing ArcGISPro](https://pro.arcgis.com/en/pro-app/latest/get-started/introducing-arcgis-pro.htm) tutorial.  Watch the short introductory video, then work through the steps.  **You will be submitting a map from this tutorial for credit.**
* *Note*, if you have trouble in "Opening the project, Step 3" for either tutorial, you can download the data for off line use instead
* When you get to "Explore Views, Step 7", double click on the map title and add your name following the video below.

<div style="overflow: hidden;
  padding-top: 56.25%;
  position: relative">
  <iframe src="Part1_Author.mp4" title="Processes" scrolling="no" frameborder="0"
    style="border: 0;
   height: 100%;
   left: 0;
   position: absolute;
   top: 0;
   width: 100%;">
   <p>Your browser does not support iframes.</p>
 </iframe>
</div>
<a href="Part1_Author.mp4" target="_blank">View Image in New Tab</a>

### Question 1)
Save the layout with your name as as Central_Wellington_Layout.pdf and upload it to the Lab1 canvas quiz.
* To save your layout reference the image below. 1) CLick Share. 2) Click Layout Export.  3) Specify the output location and name your file.  Its best to use your Lab1_Project workspace so you can easily find this when its time to submit you map.  4) Click Export.

<div style="overflow: hidden;
  padding-top: 56.25%;
  position: relative">
  <iframe src="ExportLayout.png" title="Processes" scrolling="no" frameborder="0"
    style="border: 0;
   height: 100%;
   left: 0;
   position: absolute;
   top: 0;
   width: 100%;">
   <p>Your browser does not support iframes.</p>
 </iframe>
</div>
<a href="ExportLayout.png" target="_blank">View Image in New Tab</a>


## Watching the videos
ESRI offers quite a few tutorials on ArcGIS Pro.  Feel free to work though them if you have time!  But we're just going to watch the overview videos from three tutorials to learn a bit more about what we can do with ArcGIS Pro.  Go to each of the following tutorial pages and watch the overview videos.
1) [Explore your data](https://pro.arcgis.com/en/pro-app/latest/get-started/explore-your-data.htm)
  * This tutorial shows you how you can interact with and explore data layers.
2) [Make a layout](https://pro.arcgis.com/en/pro-app/latest/get-started/add-maps-to-a-layout.htm)
  * This tutorial shows you how you can use map layouts to visualize data.
3) [Use geoprocessing tools](https://pro.arcgis.com/en/pro-app/latest/get-started/use-geoprocessing-tools.htm)
  * This tutorial shows a few of the ways you can analyze geospatial data and see how different layers interact.

## Question 2)
Need to think of something??  

# Part 2 – A Practical Example: The foundations of Epidemiology 

An early forms of [germ theory](https://en.wikipedia.org/wiki/Germ_theory_of_disease), the concept that disease transmission is driven by pathogens, emerged around the world more than 2000 years ago.  By the middle ages, Islamic physicians had formally proposed the basics of germ theory.  For example, writing about an outbreak of the bubonic plague in [1362](https://en.wikipedia.org/wiki/Ibn_al-Khatib#On_the_Plague), Ibn al-Khatib astutely pointed out:
	*"The existence of contagion is established by experience [and] by trustworthy reports on transmission by garments, vessels, ear-rings; by the spread of it by persons from one house, by infection of a healthy sea-port by an arrival from an infected land [and] by the immunity of isolated individuals."*  

Despite this knowledge European scientists physicians clung to the [miasma theory](https://en.wikipedia.org/wiki/Miasma_theory) that diseases, such as cholera, were caused by “bad air” for many centuries.  In the face of mounting evidence many doctors and public officials stubbornly refused to acknowledge that basic hygiene and sanitation could save lives.

* In one striking example is from two maternity clinics in the Vienna Maternity Hospital.  Between 1840 and 1846, maternal mortality rate was 98.4 per 1000 births in a clinic run by physicians and medical students.  While the rate in a the clinic run by midwives was only 36.2 per 1000 births.  The doctors/students started each day with postmortem examinations of deaths from the previous day, then proceeded to the maternity ward without washing their hands where the students performed vaginal examinations as part of their training (Loudon, 2013).  By contrast, the midwives didn't do postmortems or examinations.  Hand washing was mandated before entering the maternity ward in both clinics.  By 1848, the maternal mortality rate in the doctors/student clinic fell to 12.7 per 1000 births, comparable to the rate of 13.3 per 1000 births in the midwives clinic.  Yet, even with this, antisepsis wasn't more broadly introduced into obstetric practice until the 1880's.

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
