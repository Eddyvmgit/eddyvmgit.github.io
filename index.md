---
layout: page
permalink: /

---
<h1 id="Introduction" class="post-title">
        Introduction
</h1>

Before we dived into our research project, we asked ourselves: “What is San Francisco like?”, “How did it change over time?”, “What is a typical person from San Francisco thinking?” and we quickly concluded that while San Francisco has an immensely diverse culture, there is something that connects everyone from the same area. A deeply rooted characteristic that reflects the zeitgeist of the city: <b>The massive extradition of residents to gentrification.<b>

<a href="https://en.wikipedia.org/wiki/Gentrification_of_San_Francisco">https://en.wikipedia.org/wiki/Gentrification_of_San_Francisco</a>


Thus, we wanted to analyze if we find a relationship between the crime patterns of San Francisco and gentrification, which both seem to haunt the lovely people of this city. We wanted to find out whether a rise in gentrification leads to a decrease or rather an increase in the crimes in a district. Are certain crime types more affected by gentrification than others?

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



