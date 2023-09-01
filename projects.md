---
layout: page
title: projects
permalink: /projects
---

<!---
coming soon... i promise!
--->

A collection of professional and personal projects I've worked on with reflections. I plan on filling this out with more data analysis, visualization, and writing pieces. 

{% for post in site.posts %}
  ---
  {{ post.date | date_to_string }} &nbsp; &nbsp; [ {{ post.title }} ]({{ post.url }})  
  <div style="text-align: center;">
      <a href="{{- post.url -}}"><img src="{{- post.thumbnail -}}" class="align-center" style="float: left" alt=""></a>
  </div>
  {{ post.excerpt }}
{% endfor %}