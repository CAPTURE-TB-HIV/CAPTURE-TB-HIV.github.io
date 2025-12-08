---
title: Tools
layout: default
---

{% assign guides = site.data.outputs.guidance %}
{% if guides and guides.size > 0 %}

## Guidance

 {% for guide in guides %}

* <a href="{{guide.file}}">{{guide.name}}</a>

 {% endfor %}

{% endif %}

{% assign presentations = site.data.outputs.presentations %}
{% if presentations and presentations.size > 0 %}

## Presentations

 {% for presentation in presentations %}

* <a href="{{presentation.file}}">{{presentation.name}}</a>

 {% endfor %}

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