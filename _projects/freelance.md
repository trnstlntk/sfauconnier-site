---
layout: single
title: "Freelance work"
date_start: 2020
date_end: 
tags: [freelance]
excerpt: "Overview of freelance projects"
header:
  image: /assets/images/carshare.gif
  teaser: /assets/images/carshare.gif
gallery:
  - url: /assets/images/carshare.gif
    image_path: assets/images/unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 1"
  - url: /assets/images/carshare.gif
    image_path: assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
  - url: /assets/images/carshare.gif
    image_path: assets/images/unsplash-gallery-image-3-th.jpg
    alt: "placeholder image 3"
---

{{ page.date_start | date: "%Y" }}{% if page.date_end %} – {{ page.date_end | date: "%Y" }}{% else %} – {% endif %}

This page shows a selection of freelance projects I did since 2020.

RCE kennisbank

Open Topstukken

NADD

{% include gallery caption="This is a sample gallery to go along with this case study." %}

{% capture notice-2 %}
#### Read more

* [Read it here (and download a PDF)](http://www.spinster.be/web-specific-art)
{% endcapture %}

<div class="notice">{{ notice-2 | markdownify }}</div>
