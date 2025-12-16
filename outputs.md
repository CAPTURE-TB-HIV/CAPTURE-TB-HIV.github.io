---
title: Tools
layout: default
---

{% assign guides = site.data.outputs.guidance %}
{% if guides and guides.size > 0 %}

## Guidance

<ul>
 {% for guide in guides %}

<li>
 <a href="{{guide.file}}">{{guide.name}}</a>
<p>{{guide.description}}</p>
</li>

 {% endfor %}
</ul>
{% endif %}

{% assign presentations = site.data.outputs.presentations %}
{% if presentations and presentations.size > 0 %}

## Presentations

<ul>
 {% for presentation in presentations %}

<li> <a href="{{presentation.file}}">{{presentation.name}}</a>
	<p>{{presentation.description}}</p>
</li>

 {% endfor %}
</ul>
{% endif %}

{% assign papers = site.data.outputs.papers %}
{% if papers and papers.size > 0 %}

## Papers

 {% for paper in papers %}

* <a href="{{paper.url}}">{{paper.name}}</a>

 {% endfor %}

{% endif %}

## Tools

The following open source software tools are designed to make methods developed by CAPTURE more accessible.

{% include tool-section.html %}