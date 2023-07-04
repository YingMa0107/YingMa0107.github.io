---
layout: gridlay
title: "Publications"
permalink: /publications/
author_profile: true
---

# Publications

<div class="row row-cols-1 row-cols-xl-2">
{% for publi in site.data.publist %}
{% if publi.highlight == 1 %}

<div class="col mb-4">

 <div class="card h-100 d-flex flex-column justify-content-between bg-light" >
  <div class="card-body clearfix">
  <pubtit class="card-title">{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-fluid float-left w-33 d-inline-block"/>
  <p class="card-text">{{ publi.description }}</p>
  <p class="card-text"><em>{{ publi.authors }}</em></p>
  <p class="card-text text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p class="card-text"> {{ publi.news2 }}</p>
  </div>
  <div class="card-footer px-0 mx-auto text-center w-100">
  <p class="card-link text-nowrap"><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  </div>
 </div>
</div>

{% endif %}
{% endfor %}
</div>

<p> &nbsp; </p>

## Full List of publications

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
