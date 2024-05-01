---
layout: page
title: ReadingPosts
desc: "2024 Spring  UVa CS Machine Learning Lectures Organized by Given Order"
---


<p><a name="topPage"></a></p>



<table id="datatab3" summary="Table of posts" border="1">
<tr>
 <h3><b>
  <th>No.</th>  
  <th>Title</th>
  </b>
  </h3>
</tr>


  {% assign counter = 1 %}
  {% assign sorted = site.contents   %}
  {% for post in sorted %}
  <tr>
  <td>{{ counter }}</td>  
  <td><a href="#{{ counter }}">{{ post.title }} 
  </a></td>
  </tr>

  {% assign counter=counter | plus:1 %}
{% endfor %}
</table>


<div class="posts">

----  ----  
{% assign counter = 1 %}
{% assign sorted = site.contents   %}
{% for post in sorted %}


  <div class="post">
    <h1 class="post-title"><a name="{{ counter }}"></a>
      <a href="{{ site.baseurl }}{{ post.url }}">
        {{ counter }}.{{ post.title }}
      </a>
    </h1>
 
 <ul>
  {% if post.lecture %}
  <li><a href="{{ site.baseurl }}/Lectures/{{ post.lecture }}.pdf"  target="_blank">Lecture: 
  {{ post.lecture }}</a>
  </li>
  <li>Version: {{ post.lectureVersion }}</li>
  {% endif %}

  {% if post.extraContent %}
  <li>More advanced to Read: <a href="{{ site.baseurl }}/Lectures/{{ post.extraContent }}.pdf"  target="_blank">   {{ post.extraContent }} </a></li>
  {% endif %}

  {% if post.notes %}
  <li>Blog: {{ post.notes }} </li>
  {% endif %}

  {% if post.morenotes %}
  <li>Extra Notes to Read: {{ post.morenotes }} </li>
  {% endif %}

  {% if post.video %}
  <li>Lead: {{ post.video }} </li>
  {% endif %}

</ul>

  {% for temp in post.tags %}
    <a class="button" href="{{ site.baseurl }}/LecturesByTags/#{{temp | replace:" ","-" }}">{{ temp }}</a>
  {% endfor %}

<br>

<h3>Summary of Post :</h3>
    {% if post.content contains '<!--excerpt.start-->'  %}
      {{   post.content | split:'<!--excerpt.start-->' | first  }}
    {% else %}
      {{ post.content }}
    {% endif %}

  </div>
<hr>

<h3 style="color: blue;">Please click each post's URL shown below to check out its full contents. </h3>

{% assign counter=counter | plus:1 %}
{% endfor %}
</div>


<div style="position: fixed; bottom: 76px; left:10px; width: 88px; height: 36px; background-color: #FFCF79;">
<a style="position: fixed; bottom:80px; left:10px;" href="#topPage" title="Back to Top">BackTop</a>
</div>


<hr>
