---
layout: page
permalink: /

---
<h1 id="Introduction" class="post-title">
        Introduction
</h1>

Before we dived into our research project, we asked ourselves: “What is San Francisco like?”, “How did it change over time?”, “What is a typical person from San Francisco thinking?” and we quickly concluded that while San Francisco has an immensely diverse culture, there is something that connects everyone from the same area. A deeply rooted characteristic that reflects the zeitgeist of the city: <b>The massive extradition of residents to gentrification.<b>

<a href="https://en.wikipedia.org/wiki/Gentrification_of_San_Francisco">https://en.wikipedia.org/wiki/Gentrification_of_San_Francisco</a>


Thus, we wanted to analyze if we find a relationship between the crime patterns of San Francisco and its gentrification, which both seem to haunt the lovely people of this city. We wanted to find out whether gentrification leads to a decrease or rather an increase in a districts crime rate and if there are certain crime types more affected than others?

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
<h1 id="Crime Types" class="post-title">
       Crime Type Analysis
</h1>

In this part, as a last plot, we wanted to have an interactive histogram with Bokeh to assess which crimes in which districts changed the most and draw a relationship among specific crime types to the gentrification status. We divided this task to our third team-member but he did not respond shortly before submission. This is not meant as an excuse and we accept any grading, as we know that each of us should know how to create all of the plots, but still we were not able to construct a good plot in that short-time frame and we wanted to explain why the final  part of our report is not to the expected standards.

Here is our final times series plot (Though, it is not working yet):

{% include final_bokeh.html %}



