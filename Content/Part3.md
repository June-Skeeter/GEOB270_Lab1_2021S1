---
layout: default
title: Foundations of Epidemiology
nav_order: 4
---

# Foundations of Epidemiology

We are going to recreate one of the foundational studies in [Epidemiology](https://en.wikipedia.org/wiki/Epidemiology) and the closely related field of [Health Geography](https://en.wikipedia.org/wiki/Health_geography) using modern GIS techniques.

* [Dr. John Snow](https://en.wikipedia.org/wiki/John_Snow#Cholera) was a physician practicing in London where cholera outbreaks were a frequent occurrence due to poor sanitation practices.  Dr. Snow was a skeptic of the miasma theory and a proponent of germ theory.  In 1849 he proposed cholera that it was spread by fecal contaminated water, after comparing cholera rates between London districts supplied by different water companies.
* Five years later, during an outbreak in London's SoHo neighborhood in 1854, Dr. Snow was able to identify the point source of an the outbreak using a hand-sketched map.  He recorded each case of cholera in the area using a dash, and recorded each water pump with a circled dot, creating what today would be called a ‘dot map.’ By recording clusters of disease, and conducting interviews, Snow was able to trace most cases of the outbreak to a single water pump, located on Broad st.
  * Using this map, Dr. Snow was able to convince the local council to remove the pump handle and the outbreak subsided.
  * Despite this, the medical community in London continued to reject the idea Cholera was caused by fecal contamination was responsible for the spread of cholera for another twenty years.

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


# Applying Modern Methods to the 1854 Cholera Outbreak

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

# Creating the pumps layer

Using the steps outlined in the video on creating point features, we are going to create a new feature class called "Broad St. Pump" and digitize the location of the pump.  Follow the steps as outlined and refer to the video below.

**1)** Right click on SourcePoints in the catalog pane and click New > Feature Class.
* SourcePoints is a "Feature Dataset", a collection of feature classes within a geodatabase that have common properties (eg. projections)

**2)** In the new window that opens, give the new feature a name and alas, set the type to point, and click Next.
* Arc Pro does not allow Feature Classes to have certain characters (eg. spaces) in file names.  But you can set the alias to display spaces
* Feature classes can take multiple different types.  The three most common, which we will mainly be concerned with are: Points, Lines, and Polygons
  * We'll discuss the differences in detail in lecture

**3)** Add a new field called Name with type text then click Next.
* Fields allow us to store information about the features in a table.  In this case, the only information we want to store is the name.  We will encounter circumstances later where we store many attributes for each feature.

**4)** Note the Spatial Reference System then click Finish.
* Feature Datasets require that all feature classes within them have the same Spatial Reference System, so the projection is automatically set to that of the SourcePoints feature dataset (WGS 1984 Web Mercator)
  * If you aren't working in a preexisting feature dataset, this would be your chance to specify it
* We don't need to concern ourselves with the options on the next three pages for now.

<div style="overflow: hidden;
  padding-top: 56.25%;
  position: relative">
  <iframe src="NewPoint.mp4" title="Processes" scrolling="no" frameborder="0"
    style="border: 0;
   height: 100%;
   left: 0;
   position: absolute;
   top: 0;
   width: 100%;">
   <p>Your browser does not support iframes.</p>
 </iframe>
</div>
<a href="NewPoint.mp4" target="_blank">View Image in New Tab</a>

# Digitizing the Broad St. pump

Now we are going to digitize the location of the Broad St. Pump.  Follow the steps as outlined and refer to the video below.

**1)** Find the Snow_cholera_map in the CholeraOutbreak_1854.gdb, click and drag it onto the map.
* A geodatabase (.gdb) is a file management structure that is unique to ESRI products.
  * Geodatabases are used to store files in Arc Pro.  You don't have to store your data in a .gdb, Arc Pro can work with data stored in regular files as well.  But .gdb have some enhanced functionality that makes them better in some circumstances.  We'll discuss .gdb more in more detail later

**2)** Open the Edit tab and click Create, in the create pane that appears, click Broad St. Pump and choose point from the options that appear.
* The edit tab allows us to create, modify, save, and delete data among other things
* Create is used specifically to add new features to an existing feature data set.
  * Right now we're creating a single point feature.  We'll learn how to digitize lines and polygons later on in the semester.

**3)** Click on the location of the Broad St. pump as shown on Dr. Snow's original map, then save your edits.
* Zoom into the Broad St. area on the map, click on the location of the pump to add a point feature.
  * If you make a mistake, you can hit ctrl + z to undo your additions
  * **Note** Snapping is sometimes set to on by default.  It will cause the cursor to jump to the nearest feature in another layer (eg. Deaths).  It is useful in some situations, but not here.  It can be turned off by clicking snapping in the Edit tab.
* Save your edits after every change to make them permanent.

**4)** Open the attribute table and name the newly created feature "Broad St. Pump"
* You can type directly into the attribute table to edit the newly created features Name value, which is blank for now.
* Clicking a new row in the attribute table will add and "empty" feature with no spatial component.
  * You can right click on a row to delete that feature
* Save your edits to make them permanent.

<div style="overflow: hidden;
  padding-top: 56.25%;
  position: relative">
  <iframe src="Digitize.mp4" title="Processes" scrolling="no" frameborder="0"
    style="border: 0;
   height: 100%;
   left: 0;
   position: absolute;
   top: 0;
   width: 100%;">
   <p>Your browser does not support iframes.</p>
 </iframe>
</div>
<a href="Digitize.mp4" target="_blank">View Image in New Tab</a>


# Save your project.

Click Save in the top left of the Arc Pro window.
