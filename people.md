---
layout: gridlay
excerpt: "Computational Fluids Group: People"
sitemap: false
permalink: /people/
---

## Faculty

{% assign number_printed = 0 %}
{% for member in site.data.faculty %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}
<style>
.button {
  background-color: #9a9b9c; /* Gray */
  border: none;
  color: white;
  padding-top: 4px;
  padding-right: 10px;
  padding-bottom: 4px;
  padding-left: 10px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 20px;
  font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
  font-weight: 600;
  color: #ffffff;
  margin: 4px 2px;
  cursor: pointer;
}

.button1 {border-radius: 2px;}
.button2 {border-radius: 4px;}
.button3 {border-radius: 8px;}
.button4 {border-radius: 12px;}
.button5 {border-radius: 50%;}
</style>

  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="15%" style="float: left" />
  <h3>{{ member.name }}</h3>
  <i>{{ member.info }} </i><!--<br>email: <{{ member.email }}></i> -->
  <ul style="overflow: hidden; margin-top:10px;">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>

<a href = "mailto: nsharan@auburn.edu"> <button class="button button3"> Email </button> </a> 
<a href="/pdf/nek-cv-short.pdf" target="_blank"> <button class="button button3"> CV </button> </a>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


---

## Group Members
<p>   </p>
#### Graduate students

Adithya Mayya

Thiraj Wegala
<br/><br/>

#### Undergraduate students

Henry McCormick
<br/>
<br/>

 **We are actively looking for PhD, Masters and undergraduate students to join the group. Please email [Nek Sharan](mailto:nsharan@auburn.edu) for prospective positions.**
