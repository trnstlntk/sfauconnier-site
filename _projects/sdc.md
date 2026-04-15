---
layout: single
title: "Structured Data on Wikimedia Commons"
date_start: 2017-01-01
date_end: 2019-12-31
tags: [wikimedia]
excerpt: "Enhancing Wikimedia Commons with multilingual, linked data"
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

I obtained a master's degree in Art History (Licentiaat Kunstwetenschappen) at Ghent University in 1997. In that same year I handed in my thesis, quite pompously entitled Web-specific art. Het World Wide Web als artistiek medium.

It was in Dutch, it sounds a bit sweet and naive when you read it now. Probably one of its most interesting aspects, 30 years after publication, is that it contains several descriptions of interesting art projects that have been lost.

{% include gallery caption="This is a sample gallery to go along with this case study." %}

{% capture notice-2 %}
#### Read more

* [Read it here (and download a PDF)](http://www.spinster.be/web-specific-art)
{% endcapture %}

<div class="notice">{{ notice-2 | markdownify }}</div>
