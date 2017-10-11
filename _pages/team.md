---
title: Staff
permalink: /team/
layout: single
header:
  overlay_image: /assets/img/vegas.jpg
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
  caption: "Photo credit: [**dfbarrero**](https://www.flickr.com/photos/dfbarrero/)"
  #cta_label: "More Info"
  #cta_url: "https://unsplash.com"
#header:
#  video:
#	id: rQw8VGJsfCg
#	provider: youtube
---

These are videogames developed by former students that agreed to publish them.

<ol>
{% for person in site.data.team %}
    <h2>{{ person.name}} </h2>
    <p><strong>Role:</strong> {{ person.role}} <br>
    <strong>URL</strong>: {{ person.url}} <br>
    <strong>Photo</strong>: {{ person.photo}} </p>

    <br>
{% endfor %}
</ol>


