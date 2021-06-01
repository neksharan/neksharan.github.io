---
title: ""
layout: gridlay
excerpt: "Computational Fluid Group -- Research."
sitemap: false
permalink: /research/
bigimg:
  - "/img/CylVort_LineCont1_cropped_copy1.png"
---

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% if publi.highlight == 1 %}

<div class="well">
  <img src="{{ site.url }}{{ site.baseurl }}/images/respic/{{ publi.image }}" class="img-responsive" width="30%" style="float: left" />
  <pubtit>{{ publi.title }}</pubtit>
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% endif %}
{% endfor %}

<p> &nbsp; </p>