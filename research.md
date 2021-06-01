---
title: "Research"
layout: page_research
excerpt: "Computational Fluid Group -- Research."
sitemap: false
permalink: /research/
bigimg:
  - "/images/respic/CylVort_ResearchWebpage_copy.png"
---

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% if publi.highlight == 1 %}

<div class="well">
  <img src="{{ site.url }}{{ site.baseurl }}/images/respic/{{ publi.image }}" class="img-responsive" width="30%" style="float: left" />
  <pubtit>{{ publi.title }}</pubtit>
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link1.url }}" target="_blank">{{ publi.link1.display }}</a></strong></p>
  <p style="margin-top:-1.5em"><strong><a href="{{ publi.link2.url }}" target="_blank">{{ publi.link2.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% endif %}
{% endfor %}

<p> &nbsp; </p>

<b> <font size="+2"> and more ... </font> </b>