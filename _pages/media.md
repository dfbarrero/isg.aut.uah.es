---
title: Media
layout: single
permalink: /media/
header:
  overlay_image: /assets/img/farolillos.jpg
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
  caption: "Photo credit: [**dfbarrero**](https://www.flickr.com/photos/dfbarrero/)"
  #cta_label: "More Info"
  #cta_url: "https://unsplash.com"
---

<h2 class="bibliography">Press</h2>

<ul class="bibliography">
{% for media in site.data.media %}
{% if media.type == "press" %}
    <li>
         <i><a href="{{media.url}}">{{media.title}}</a></i>. {{media.media}} ({{media.date}})
    </li>
{% endif %}
{% endfor %}
</ul>

<h2 class="bibliography">Radio</h2>

<ul class="bibliography">
{% for media in site.data.media %}
{% if media.type == "radio" %}
    <li>
         <i><a href="{{media.url}}">{{media.title}}</a></i>. {{media.media}} ({{media.date}})
    </li>
{% endif %}
{% endfor %}
</ul>

<h2 class="bibliography">Specialized media</h2>

<ul class="bibliography">
{% for media in site.data.media %}
{% if media.type == "special" %}
    <li>
         <i><a href="{{media.url}}">{{media.title}}</a></i>. {{media.media}} ({{media.date}})
    </li>
{% endif %}
{% endfor %}
</ul>


