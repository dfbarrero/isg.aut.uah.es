---
title: Projects
layout: single
permalink: /projects/
header:
  overlay_image: /assets/img/a350.jpg
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
  caption: "Photo credit: [**dfbarrero**](https://www.flickr.com/photos/dfbarrero/)"
  #cta_label: "More Info"
  #cta_url: "https://unsplash.com"
---

<iframe width="560" height="315" src="https://www.youtube.com/embed/6cSWPd1M_pA" frameborder="0" allowfullscreen></iframe>
<br>

<h2 class="bibliography">National projects</h2>

<ol class="bibliography">
{% for project in site.data.projects %}
{% if project.type == "National" %}
    <li>
			{% if project.url %}
				<a href="{{project.url}}" style="text-decoration:none;"><i>{{ project.name}}</i></a>. {{ project.funding}}. Participation of {{ project.participants}}. PI: {{ project.pi}}. {{project.grant}}. {{ project.years}}.
			{% else %}
				<i>{{ project.name}}</i>. {{ project.funding}}. Participation of {{ project.participants}}. PI: {{ project.pi}}. {{project.grant}}. {{ project.years}}.
			{% endif %}
	</li>
{% endif %}
{% endfor %}
</ol>

<iframe width="560" height="315" src="https://www.youtube.com/embed/iRlg25wF6jw" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<h2 class="bibliography">International projects</h2>

<ol class="bibliography">
{% for project in site.data.projects %}
{% if project.type == "International" %}
    <li>
		{% if project.url %}
			<a href="{{project.url}}"><i>{{ project.name}} </i>. {{ project.funding}}. Participation of {{ project.participants}}. PI: {{ project.pi}}. {{project.grant}}. {{ project.years}}.</a>
		{% else %}
			<i>{{ project.name}} </i>. {{ project.funding}}. Participation of {{ project.participants}}. PI: {{ project.pi}}. {{project.grant}}. {{ project.years}}.
		{% endif %}
	</li>
{% endif %}
{% endfor %}
</ol>


