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
 
 /*
	From this point onwards, the CSS code refers to 
	how to create and manage flipable cards.
 */
 .flip-card {
  background-color: transparent;
  width: 300px;
  height: 300px;
  perspective: 1000px;
}

.flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 0.6s;
  transform-style: preserve-3d;
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
}

.flip-card:hover .flip-card-inner {
  transform: rotateY(180deg);
}

.flip-card-front, .flip-card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
}

.flip-card-front {
  background-color: #ffffff;
  color: black;
}

.flip-card-back {
  background-color: #ffffff;
  color: black;
  transform: rotateY(180deg);
}

</style>

{% assign count = 0 %}

{% for person in site.data.team %}
 {% assign odd = count | modulo:2 %}
 {% if odd == 0 %} <div class="row"> {% endif %}
 
  <div class="column">
	<a href="{{person.url}}">
	<!-- flip-card classes refer to the flipping card elements-->
		<div class="flip-card">
		  <div class="flip-card-inner">
			<div class="flip-card-front">
			  <img src="{{site.url}}/{{site.baseurl}}/{{ person.photo }}" alt="{{ person.name }}" style="height:100%">
			</div>
			<div class="flip-card-back">
			  <h1>{{ person.name }}</h1> 
			  <p class="title">{{ person.role }}</p>
			  <p>{{ person.interest }}</p>
			</div>
		  </div>
		</div>
	</a>
  </div>
 {% if odd != 0 %} </div> {% endif %}

   {% assign count = count | plus: 1 %}
{% endfor %}

