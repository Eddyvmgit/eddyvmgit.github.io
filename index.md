---
layout: page
permalink: /

---
<h1 id="Introduction" class="post-title">
        Introduction
</h1>

New York is a vibrant and busy city, but the greatness of the city comes with a great expense: <b>a high density of traffic accidents</b>. This is an important public safety issue, especially in a city where “on average, three people die every day due to a traffic-related crash.' In this article, we aim to examine New York's traffic accident patterns in detail, using statistical analysis to uncover dangerous intersections and gain valuable insights into what is going wrong. By analysing the data, our goal is to understand the factors contributing to these accidents locally, and suggest practical recommendations to improve traffic safety. With our story we hope to raise awareness of dangerous traffic patterns and motivate city planners to design safer environments.

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

We analysed the different intersections of New York and attempted to highlight local properties that lead to a high accident and injury rate. Furthermore, we proposed solutions, while also giving the reader of this article the chance to make his own discoveries in regards to the 10 most dangerous intersections of New York based on the total number of accidents. Lastly, we analysed the accident patterns by year, month, day and hour to find specific patterns for which we proposed further solutions. 



