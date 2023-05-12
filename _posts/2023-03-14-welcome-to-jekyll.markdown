---
layout: post
title:  "Looking for Accident Hotspots"
date:   2023-05-12 11:23:50 +0100
number: "2"
categories: jekyll update
---

First, we clustered all accident records from the dataset according to their geographical position to group them at an intersection level. Below is a map of the 10th most dangerous intersections according to the absolute accident number from 2013-2022 in New York. The color intensity of each cluster indicates the number of injured people due to traffic-related accidents at each intersection. Notably, the darkest cluster on the map corresponds to the intersection of 9th Avenue with W 41 Street, including over 504 injuries and 1195 total accidents during 2013-2022. The size of each cluster indicates the total number of accidents.

Here we can see that cluster 707 had 1351 accidents in the same time interval but only 156 injuries. As we now found the most dangerous areas, we can dive deeper into each cluster and analyze the local properties that lead to their high density of accidents.

{% include map_final.html %}

It is important to note that these clusters are most likely referring to intersections having the highest traffic volume, as we expect traffic volume to be strongly correlated with the number of accidents. Unfortunately, Mapbox does only provide traffic volume data to institutions [1]. However, when comparing the clusters noted before, the former included a much higher rate of injuries than the latter one, even though their accident rate is comparable. This shows that the corresponding intersections have different traffic-related properties making one more dangerous than the other, regardless of their traffic volume.

[1] <a href="https://www.youtube.com/watch?v=T3MCOjdgBSk&ab_channel=KuanButts">Reference Video</a>

