---
layout: page
title: ReadingPosts
desc: "2022 Spring  UVa CS Machine Learning Lectures Organized by Given Order"
---


<p><a name="topPage"></a></p>

<div class="posts">

----  ----  
{% assign sorted = site.contents   %}
{% for post in sorted %}

  <div class="post">
    <h1 class="post-title">
      <a href="{{ site.baseurl }}{{ post.url }}">
        {{ post.title }}
      </a>
    </h1>
 
 <ul>
  {% if post.lecture %}
  <li><a href="{{ site.baseurl }}/Lectures/{{ post.lecture }}.pdf"  target="_blank">Lecture: 
  {{ post.lecture }}</a></li>
  <li>Version: {{ post.lectureVersion }}</li>
  {% endif %}

  {% if post.extraContent %}
  <li>More advanced to Read: <a href="{{ site.baseurl }}/Lectures/{{ post.extraContent }}.pdf"  target="_blank">   {{ post.extraContent }} </a></li>
  {% endif %}

  {% if post.notes %}
  <li>Notes to Read: {{ post.notes }} </li>
  {% endif %}

  {% if post.morenotes %}
  <li>Extra Notes to Read: {{ post.morenotes }} </li>
  {% endif %}

  {% if post.video %}
  <li>Video: {{ post.video }} </li>
  {% endif %}

</ul>

  {% for temp in post.tags %}
    <a class="button" href="{{ site.baseurl }}/LecturesByTags/#{{temp | replace:" ","-" }}">{{ temp }}</a>
  {% endfor %}

<br>


  {% if post.lecture  %}
    {% if post.lectureVersion contains 'current' %}

    {% endif %}
  {% endif %}

    {{ post.content }}


  </div>
<hr>

{% endfor %}
</div>


<div style="position: fixed; bottom: 76px; right:10px; width: 88px; height: 36px; background-color: #FFCF79;">
<a style="position: fixed; bottom:80px; right:10px;" href="#topPage" title="Back to Top">BackTop</a>
</div>


<hr>
