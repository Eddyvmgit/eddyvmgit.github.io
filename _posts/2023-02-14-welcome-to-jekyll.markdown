---
layout: post
title:  "Finding Patterns in Time"
date:   2023-05-10 11:23:50 +0100
number: "4"
categories: jekyll update
---

We took a step back to study the general data in order to discover certain time trends. Below are the related plots. The first plot shows the total number of accidents per month for each year. A noteworthy observation is that there is one year, 2020, that follows a trend different from the rest of the years. The drop in incidents during this year can be attributed to the entry of COVID-19 and subsequent lockdown measures that restricted activity in major cities like New York. For the other years, they all follow a general trend of having fewer incidents during the winter months than during the summer months. This could be explained by the fact that people tend to engage in more activities during the summer than during the winter. It is recommended that users take extra precautions during the summer months.

![image tooltip here](/assets/final_dist_plot.png)

We wanted to have a deeper look into the covid related traffic patterns. The following heatmaps compare the distribution of incidents during the years 2022, 2021 and 2020, that were unusual due to the COVID-19 pandemic and the lockdown.

![image tooltip here](/assets/rona_1.png)
![image tooltip here](/assets/rona_2.png)
![image tooltip here](/assets/rona_3.png)

The intensity of the squares indicates a higher accumulation of incidents. We can see that 2022 and 2021 follow the normal distribution as every year, with more accidents generally concentrated during the summer months. In 2020, it can be seen that the pattern changes radically, with more incidents accumulating before and after the lockdown measures, and a huge gap in intensity during the lockdown.

This is in a great accordance to the implemented lockdown in New York that started March 30th:

<a href="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8806179/#:~:text=NYC%20implemented%20its%20lockdown%20on,1%E2%80%935%20AM%20for%20cleaning.">Lockdown Article</a>


The below illustration represents the hourly traffic density distributed over the days of the week. In the heatmap, it can be seen the two heat zones that symbolise the two peaks found in the first representation. One around 8 o'clock and the other around 17 o'clock, which makes sense given the fact that most people commute to and from work during these hours. We can also see that the weekend breaks this cycle, showing less traffic accidents during these hours and a higher rate at and past midnight. Regarding these late-night accidents, we would propose to establish speed limit zones past midnight on the weekend, around the relevant intersections where these accidents typically occur. 

![image tooltip here](/assets/final_heat_plot.png)
