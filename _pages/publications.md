---
layout: gridlay
title: "Publications"
permalink: /publications/
author_profile: true
---

<style>
.image-margin {
  margin-bottom: 20px;
  margin-left: 20px;
}

.text-margin {
  margin-top: 20px;
  margin-left: 20px;
}
</style>

# Publications
{% if page.header.overlay_color or page.header.overlay_image or page.header.image %}
  {% include page__hero.html %}
{% endif %}

{% if page.url != "/" and site.breadcrumbs %}
  {% unless paginator %}
    {% include breadcrumbs.html %}
  {% endunless %}
{% endif %}

<div class="container">
  <div class="row row-cols-1 row-cols-md-2">
    {% for publi in site.data.publist %}
      {% if publi.highlight == 1 %}
        <div class="col mb-4">
          <div class="card h-100 d-flex flex-column justify-content-between bg-light">
            <img src="{{ site.url }}{{ site.baseurl }}/images/{{ publi.image }}" class="card-img-top image-margin" alt="{{ publi.title }}">
            <div class="card-body" style="text-align: justify;">
              <h5 class="card-title">{{ publi.title }}</h5>
              <p class="card-text text-margin">{{ publi.description }}</p>
              <p class="card-text text-margin"><em>{{ publi.authors }}</em></p>
              <p class="card-text text-margin text-danger"><strong>{{ publi.news1 }}</strong></p>
              <p class="card-text text-margin">{{ publi.news2 }}</p>
            </div>
            <div class="card-footer">
              <a href="{{ publi.link.url }}" class="card-link text-nowrap"><strong>{{ publi.link.display }}</strong></a>
            </div>
          </div>
        </div>
      {% endif %}
    {% endfor %}
  </div>

  <p>&nbsp;</p>

  <h2>List of publications</h2>
  {% for publi in site.data.publist %}
    <p>
      {{ publi.title }}<br>
      <em>{{ publi.authors }}</em><br>
      <a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
    </p>
  {% endfor %}
</div>
