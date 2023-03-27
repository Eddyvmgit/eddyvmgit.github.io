---
layout: page
permalink: /

---
<h1 id="Introduction" class="post-title">
        Introduction
</h1>

In our work analyzing crime s data for San Francisco, we know that it is a city that is growing by leaps and bounds. So we wanted to introduce you to an interesting question in terms of how there is a relationship between crime type, crime frequency, and gentrification when it comes to gentrifications, and whether it is influenced by some landmark events and trends in the city. We want to see what this sample data shows us.

It's funny how things start, as two words we hear a lot in the news lately are economy and crime. As we scrolled through the pages the other day, we saw the collapse of Silicon Valley Bank, and all the voices seemed to be telling us a new financial crisis was coming. So we searched curiously for news about the serious, global financial crisis of 2008, and in it, we came across this interesting story from Washington (Reuters). In the article, the U.S. police chief said that "the recession is fueling a rise in crime" and mentioned that "the link between crime and the economy has long been controversial. "This makes us curious about this crime data for San Francisco, whether gentrification causes changes in crime in a region, and whether there is any connection between them.

In a further search on San Francisco's development, we found that in 2012, San Francisco released the Central Market Economics Strategy, which mentioned plans to redevelop the Central Market and adjacent land in the downtown area. Shortly thereafter, in early 2013, the San Francisco News published a story stating that "San Francisco's crime rate has reached a five-year high". And the article stated, "The Southern area has also been transformed and enriched by the city's booming tech sector, which has helped lower the city's unemployment rate to 5.3 percent." This raises even more curiosity about the growth of the city, the growth of the industry on how people live and the crime situation.

Combining the information from the articles we searched, we wanted to be able to classify the data by time and geographic location according to the degree of gentrification, and then perform further data analysis by comparing their heat maps. Based on the timing of the important events of the articles, we divided the data into three stages of gentrification, 2003-2007, 2008-2012, 2013-2018, and then grouped the crime data according to the different stages, and finally created heat maps and compared them on the map.


<div class="posts">
  {% for post in site.posts %}
  <div class="post">
    <h1 id = '{{ post.title }}' class="post-title">
        {{ post.title }}
    </h1>

    <span class="post-date">{{ post.date | date_to_string }}</span>

    {{ post.content }}
  </div>
  {% endfor %}
</div>
<h1 id="Conclusion" class="post-title">
        Conclusion
</h1>