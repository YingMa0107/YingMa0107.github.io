---
layout: gridlay
title: "Publications"
permalink: /publications/
author_profile: true
---

# Publications
{% if page.header.overlay_color or page.header.overlay_image or page.header.image %}
  {% include page__hero.html %}
{% endif %}

{% if page.url != "/" and site.breadcrumbs %}
  {% unless paginator %}
    {% include breadcrumbs.html %}
  {% endunless %}
{% endif %}

{% include publications.html %}
