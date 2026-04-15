---
layout: single
title: "ARTtube"
date_start: 2011
date_end: 2013
tags: [web],[video]
excerpt: "I probably wrote the world’s first thesis about internet art."
header:
  image: /assets/images/arttube.png
  teaser: /assets/images/arttube.png
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

Between 2011 and 2013 I was project lead for ARTtube, a video platform and website for Dutch and Belgian museums. ARTtube started as the video channel of Rotterdam's Museum Boijmans Van Beuningen, and grew in 2011 to become a collaborative project. It existed until 2019.

In 2014 I got the opportunity to become Wikimedian in Residence for Stichting Academisch Erfgoed, but I stayed connected to ARTtube as a freelancer. I became interested in videomaking as well, and did video production for several years.

{% include gallery caption="This is a sample gallery to go along with this case study." %}

{% capture notice-2 %}
#### Read more

* (arttube.nl over time)[https://web.archive.org/web/*/www.arttube.nl] - archived in the Internet Archive's Wayback Machine
* (Boekman Extra #14: ARTtube)[https://www.boekman.nl/verdieping/boekman-extra-14-arttube/], March 2019 (in Dutch) - a postmortem about the project, by Edo Dijksterhuis
{% endcapture %}

<div class="notice">{{ notice-2 | markdownify }}</div>
