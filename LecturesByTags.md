---
layout: page
title: ReadingByTag
desc: "2024 Spring  UVa CS Machine Learning Lectures Organized by Tags"
---
<p><a name="topPage"></a></p>


Click on a tag to see relevant list of lectures.

<ul class="tags">
{% assign tags =  site.contents | map: 'tags' | uniq | sort %}
{% for tag in tags %}
  {% assign t = tag  %}
  <li><a href="{{ site.baseurl }}/LecturesByTags/#{{t | replace:" ","-" }}">{{ t }}</a></li>
{% endfor %}
</ul>

---

{% assign tags =  site.contents | map: 'tags' | uniq | sort %}
{% for tag in tags %}
  {% assign t = tag %}

<h1><a name="{{t | replace:" ","-" }}"></a><a class="internal" href="{{ site.baseurl }}/LecturesByTags/#{{t | replace:" ","-" }}">{{ t  }}</a></h1>

<!--- for each tag, get a table of index -->


<table id="datatab3" summary="Table of Lectures" border="1">
<tr>
 <h3><b>
  <th>Title</th>
  <th>Lecture</th>
  </b>
  </h3>
</tr>


  {% assign counter = 1 %}
  {% for post in site.contents %}
    {% if post.tags contains tag %}
 
  <tr>

  <td><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }} </a></td>

  {% if post.lecture %}
  <td><a href="{{ site.baseurl }}/Lectures/{{ post.lecture }}.pdf"  target="_blank">SlideDeck</a></td>
  {% else %}
  <td></td>
  {% endif %}


  </tr>

  {% assign counter=counter | plus:1 %}
  {% endif %}
{% endfor %}
</table>

<!--- for each tag, present its posts in orders -->


{% endfor %}


<div style="position: fixed; bottom: 76px; left:10px; width: 88px; height: 36px; background-color: #FFCF79;">
<a style="position: fixed; bottom:80px; left:10px;" href="#topPage" title="Back to Top">BackTop</a>
</div>
