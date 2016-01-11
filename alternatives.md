---
layout: page
title: Alternatives Beyond Psychiatry
permalink: /alternatives/
---

<div class="posts">
  {% for post in paginator.posts %}
    <article class="post">    
      
      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="content">
        {{ post.content | truncatewords:60 }}
        <div class="date">
          Posted on {{ post.date | date: "%B %e, %Y" }}
        </div>
      </div>
      
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>


{% include /pagination.html %}
