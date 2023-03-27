---
layout: post
title:  "Does gentrification lead to an increase or decrease of crimes within a district?"
date:   2023-03-27 11:23:50 +0100
number: "2"
categories: jekyll update
---

To answer this question, we planned to create a map plot that, on the one hand, visualizes the increase of the crime rate over the years for each district while also visualizing its status of gentrification in the relevant time interval.

A quick search on the web led us to the following site: 

<a href="https://www.urbandisplacement.org/maps/sf-bay-area-gentrification-and-displacement/">https://www.urbandisplacement.org/maps/sf-bay-area-gentrification-and-displacement/</a>

Here, researchers of the urban displacement project analyzed housing market dynamics, and displacement- and gentrification statistics from 2000 to 2018 to create an interactive gentrification and displacement typology map on a sub-district/neighbourhood level of San Francisco. Each sub-district/neighbourhood was classified with one of the following typologies indicating their status of gentrification: 

<img style="max-width: 300px" src="{{ site.baseurl }}assets/labels.png">

We downloaded the relevant typology classifications incleading the geological data from this link: 
<a href="https://github.com/urban-displacement/displacement-typologies
">https://github.com/urban-displacement/displacement-typologies
</a>

However, the gentrification data is on a sub-district/neighbourhood level while the crime dataset utilised a district level. To combine both datasets, we used a python library called "shapely" to classify the smaller neighbourhoods of the gentrification dataset within the bigger districts of the crime dataset based on the geo-locations retrieved from the relevant geoJSON files. Whereafter, each district contained the typologies of all its sub-neighbourhoods, for which we used the most frequent typology

As an example, the district "Southern" had three classified neighbourhoods that included the following typologies: ["Early/Ongoing Gentrification", "Early/Ongoing Gentrification", "Advanced Gentrification"], which led us to classify the district as "Early/Ongoing Gentrification".

After retrieving the typologies, we wanted to see how the crime rate evolved in each district. Here, we fitted a linear regression line to the yearly crime increase from  2002-2017 and used its weight coefficient as the measure of crime growth in that interval. We used the Choropleth map from Plotly to visualize the data in the plot below. 

{% include gen_map.html %}

Looking at the map plot, we can see that the districts Nothern, Central and Southern had a relatively high increase in crime rate over the years. Furthermore, these districts were classified as either becoming exclusive or as being in a state of early/ongoing gentrification. On the other hand, most other districts were classified as either being stable with a moderate/mixed-income or with a low income and a suspicion of future displacement. The crime rates in these districts were either constant or even decreased during the relevant years. This indicates that the acute process of gentrification and the aftermath of exclusivity could be related to an increase in crime rate, while more stable districts with low/mixed-income experience are likely to experience a drop in their crime rate. However, it is to note that these results should be analyzed with caution, as we aggregated the data from neighbourhoods and approximately classified the enclosing district, while there could be a lot more factors other than gentrification contributing to this result. 