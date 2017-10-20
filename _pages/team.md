---
title: Staff
permalink: /staff/
layout: single
header:
  overlay_image: /assets/img/vegas.jpg
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
  caption: "Photo credit: [**dfbarrero**](https://www.flickr.com/photos/dfbarrero/)"
---

<style>

 /* Three columns side by side */
 .column {
    float: left;
    width: 50%; 
    margin-bottom: 16px; 
    padding: 0 8px;
 }

 /* Display the columns below each other instead of side by side on small screens */
 @media (max-width: 650px) {
    .column {
        width: 100%; 
        display: block; 
    }
 }

 /* Add some shadows to create a card effect */
 .card {
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2); 
 }

 /* Some left and right padding inside the container */
 .container {
    padding: 0 16px;
 }

 /* Clear floats */
 .container::after, .row::after {
    content: "";
    clear: both;
    display: table;
 }

 .title {
    color: grey;
 }

</style>

{% assign count = 0 %}

{% for person in site.data.team %}
 {% assign odd = count | modulo:2 %}
 {% if odd == 0 %} <div class="row"> {% endif %}
 
  <div class="column">
    <div class="card">
      <a href="{{ person.url }}">
      <img src="{{site.url}}/{{site.baseurl}}/{{ person.photo }}" alt="{{ person.name }}" style="width:100%">
      </a>
      <div class="container">
        <h2>{{ person.name }}</h2>
        <p class="title">{{ person.role }}</p>
        <p>{{ person.interest }}</p>
      </div>
    </div>
  </div>
 {% if odd != 0 %} </div> {% endif %}

   {% assign count = count | plus: 1 %}
{% endfor %}

