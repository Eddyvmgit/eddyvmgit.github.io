---
layout: page
permalink: /

---
<h1 id="Introduction" class="post-title">
        Introduction
</h1>
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