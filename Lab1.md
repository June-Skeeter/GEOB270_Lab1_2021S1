# Introduction 

In Part I this lab you will be introduced to ESRI's ArcGIS Pro software by several tutorials on the ESRI website. In Part II we'll do a quick example, applying modern GIS methods to a foundational study in Epidemiology.

## Learning Objectives

•	Learn about different data types 
•	display map features 
•	add data to your map 
•	manipulate data tables 
•	create a map (layout) 
•	save your map and associated data files 
•	Learn how data can be created through digitizing
•	Create a raster layer from a vector layer
•	Explore a foundational study in epidemiology


## Setting Up & Saving Your Work

* See the Lab Details page for information on how to access ArcPro using your own computer or a Geography Department computer.

* If you are using ArcPro installed on your own computer, you can manage your files however works best for you.  However, if you are working on a Geography lab computer, follow the instructions on the lab details page closely.



# Part 1: A “Quick Start” to ArcGIS Pro Software 

Demonstrate basic use of GIS software ArcGIS Pro by completing 3 ArcGIS Pro “Quick Start” tutorials from ESRI (Environmental Systems Research Institute).  The following tutorials will give you a brief overview of the skills you will be building on each lab. By the end of the term you will have become comfortable utilizing these GIS skills/tools. The three tutorials will take you about 1:40 minutes all together:

* Introducing ArcGISPro ~ 25 minutes
* Explore your data ~ 45 minutes
* Author a Map ~ 30 minutes


## Step 1: Setting up the ESRI campus access 

* Using your favorite web browser, follow this [link](http://www.esri.com/training/main) to access the ESRI training website.
* Under the top navigation bar click on Sign in. **If you have purchased ArcGIS Pro, you can sign in through your UBC ArcGIS online account. If you are using the lab computers, and don’t already have one, ‘create a new public account’**. 
* Once signed in, navigate to the ArcGIS Pro Quick Start Tutorial web page. 
* You will be sent your account email, check your spam if you do not get it right


## Step 2: "Introducing ArcGISPro" (Tutorial 1) 
On the left side of your screen, click Learn the basics tab you’ll be redirected to the Introducing ArcGIS Pro page. Watch the Video and then work your way through the tutorial. You will get points by demonstrating your completion of the tutorial by completing the following checkpoints. 
**It is highly recommended you complete these checkpoint questions during or immediately after your completion of the tutorial**. 
1)	Click on the Central Wellington_3d Map and hold down until the docking icon appears. Dock it to the right side of the screen. In the Bookmarks tab click on ‘Jervois Quay’ so that both maps zoom to that view. Upload a screenshot with both the Wellington City basemap (left) and Central Wellington_3d in side by side view. 
2)	Toggle to the Central Wellington Map. Open the Buildings attribute table, what is the 
‘Maximum Direct Solar Radiation’ of the building with an ‘OBJECTID’ of 14? (Just after Step 6 under the section Working with Contextual Tabs).  


## Step 3: "Explore your Data Tutorial" (Tutorial 2) 
Now click the the ‘Explore your data’ tab under Learn the Basics. To the right you can see a list of core GIS skills this tutorial will cover. Watch the video and begin to work your way through the tutorial. Complete the following checkpoints/questions as you work through it. 
3)	In the New Zealand Map, click on the ‘Canterbury’ region. What is the area in (square kilometers) of this region? (After Step 3, under Explore the regions and their attributes) 
4)	Open the attribute table for ‘Regions’ and locate the Sheep_2014 Column, using the Sort Ascending tool, report which region had the fewest sheep in 2014, and what the total population was in that region.  
5)	In the Regions Table right click the row with Tasman listed under region, and click pop-up. Take a screenshot of your full ArcGISPro window, demonstrating the altered alias names (e.g. ‘Area in Square Km instead of Aea_SQ_KM) that you changed in the steps above. (After Step 16, In the ‘Design Fields’ section) 
6)	When Calculating the Summary Statistics for the South Island of new Zealand try changing the Statistic Type to Mean, rename the output to south_island_statistic_mean. Check the results, what is the mean number of Beef Cattle on the South Island in 2014? (After step 13 under Summarize Table Values). 
7)	In the ‘Fields’ section, select Sheep 1994 instead. Relabel the Y axis as Number of Sheep. X axis should still be Region Name, and Title- New Zealand Sheep by Region in 1994. Upload a screenshot of your ArcGISPro window including your Chart of the Distribution of Sheep by region in 1994. (Complete after ‘Chart Sheep Distribution by region’). 
 

## Step 4: "Author a map Tutorial" (Tutorial 3) 
Now Scroll click the ‘Author a map’ tab under the Learn the Basics. Watch the video and then complete the tutorial. Complete the following checkpoints/questions as you go along. 
*Note: The Author A Map Data weblink is broken. The correct link is:*
https://www.arcgis.com/home/item.html?id=0c9ce6476eba401bb9a4affd9ae2ccbe
Downloading and saving your map 
Extract data from Downloads to the C:/temp folder. 
Save your project to the C:/temp folder as well (REMINDER: Move your work to your personal H:/ drive when done for the day) 
8)	Open the metadata for DOC tracks, who are these data credited to (full name)? And what is the purpose of the data? 
9)	Open the attribute table for your new North New Zealand trails layer. What type of vector/shape are these features? 
10)	Using your map and attribute data, what are the names of three tracks within 150 meters of mangroves? How did you find this out? 
11)	Test out some different colors for symbology of the trails and mangroves, zoom out so that the North Island is centered in the map frame. Take a screenshot of your work and upload it here. 


# Part 3 – A Practical Example: The foundations of Epidemiology 

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

We're going to work with Dr. Snow's original data and replicate the study using modern GIS methods.  In order to get the map into a GIS, it has to be scanned and then georeferenced.  To georeference a map like this, points on the scanned map (eg. intersections) can be matched up to an existing map.  With enough points, an accurate transformation can be calculated and the map can be projected.  Once the map has been scanned and georeferenced, we can extract information from it.  On Dr. Snow’s map, the key pieces of information are the cholera deaths and water pumps.

Adding and Editing the Data

The map is already georeferenced for you and the point data has already been extracted.

•	In the top left, under the insert tab, click New Map
o	As in Part 2, rename the new map Part 3
•	Under the View tab, click Catalog Pane.  This will dock the Catalog Pane on the right side of your window, showing a file tree.  Your window should now look something like the image below.
•	You now know two ways to access the Catalog.  The Catalog window and the Catalog pane.  The Catalog window shows more detailed information, allowing you to inspect the metadata.  While the Catalog Pane just shows the file tree and is a quick way to navigate folders and add data.
•	In the Catalog Pane, under Folders/lab2_data expand the CholeraOutbreak_1854.gdb
o	Click on Snow_cholera_map and drag it onto your Part 3 map area.  The scanned map from Dr. Snow’s original work should load, and the map area will be centered on the Soho neighborhood of London. Your map should now look like show below.  Toggle the Snow_cholera_map on and off to see how things in Soho look now compared to 1854.


### Screenshot 1





# References

Loudon, I. (2013). Ignaz Phillip Semmelweis’ studies of death in childbirth. Journal of the Royal Society of Medicine, 106(11), 461–463. https://doi.org/10.1177/0141076813507844
