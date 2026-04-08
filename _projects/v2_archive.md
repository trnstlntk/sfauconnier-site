---
layout: single
title: "MA thesis: Web-Specific Art"
date_start: 1996
date_end: 1997
tags: [art history]
excerpt: "I probably wrote the world’s first thesis about internet art."
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


I fully quote a rather technical project description, written by Pieter van Kemenade, who was the project’s main developer during that period.
However, much of the richness of the  cloudlike structure of the archive has been sacrificed in that export to gain simplicity and ease of use. The archive backed up here is a typical example of a 2000-ish object-relational cloud-like approach to data structures, where the archive’s structure is trying to mimic reality as close as possibly. The design by Enric Gili Fort clearly reflects that approach.
In practice, it was a PITA to maintain and develop applications on – but in its final form, the XMLServlet was able to generate fully OWL-compatible RDF as early as 2006, which was a remarkable achievement.
"Content

The content was maintained by Sandra Fauconnier (aka Fokky) and Rens Fromme using first Filemaker, then the custom solution called v2o, then MMbase. After Sandra and Rens left V2_, Arie Altena took up  content management for the archive site."
DEAF98 (the art of the accident) was still based on the Filemaker database. DEAF2000 was the first  site presented using MMBase and JSP. It was designed by Melanie Kandelaars; Jan Wijbrand Kolman and Carlo  E. Prelz did technical support, P. van Kemenade (aka pike) built the html.
From DEAF2000 onwards, the “main” v2_ site was replaced by a “interim” design by Melanie Kandelaars, pending a new design based on MMBase. Such a design was created by Nirit Peled; the process was managed by Maarten Handstede. P. van Kemenade built it, in 100% Flash and XML, but its performance was so slow and heavy on client machines it was never launched publicly. At this point it was decided to separate the main v2_ site from an “archive site”, both yet to be build.
The archive represents  all V2_’s activities and a couple of related collections, like the Daan van Golden archive. It contains text, images, and links to audio and video on the V2_ streaming servers.
One of the offsprings of the ‘flash’ effort was the ability to export XML “clusters” of data from MMBase, reflecting the types of relations that were specific to v2_’s datastructure. For that purpose, an “XMLServlet” and a “GFXServlet” were built to serve as a general backend for any V2_ webproject. A few DEAF websites have been built on this setup.
The semantic richness of V2_Archive was extremely special – and complex. We were very much ahead of our time by building a system with OWL-compatible RDF as early as 2006; this was before Linked Data really took off. I once read: when you are too early, you are wrong. But it was amazing to innovate to such an extent, even if our work was not widely known or acknowledged.
"To be continued

After launching the archive site in 2004, V2_ finally  rebuild its main website using a different technology and not using MMBase. This created a gap between the ‘main’ site and the ‘archive’ site, which wasnt solved until the main site was rebuild using Plone by Rui Guerra and Piem Wirtz in 2008. In 2010 the XML servlet’s backend was used for the last time to create RDF exports of the  MMBase data to import into Plone, so the data has not been lost."
"Much more info about the history of V2_Archive on V2_’s current website: http://v2.nl/archive/works/v2_archive

And my profile and publications during that time: http://v2.nl/archive/people/sandra-fauconnier"
I was archivist for V2_ Institute for the Unstable Media from 2000 till 2007. V2_ is a cultural organisation in Rotterdam that focuses on electronic art. Around 2000, the organisation started to structurally document and organize its very interesting history in a formal archive database and website.
In 2003, a design for the archive site was made by Enric Gili Fort and implemented by P. van Kemenade  and Jasper op den Coul. The information collected from MMBase by the XMLServlet was transformed using XSLT/python into webpages. This is the site that is backed up here.

The complete history described above, from Filemaker to XMLServlet, was managed by Boudewijn Ridder, who left V2_ to join the Nederlands Fotomuseum shortly after.

{% include gallery caption="This is a sample gallery to go along with this case study." %}

{% capture notice-2 %}
#### Read more

* [Read it here (and download a PDF)](http://www.spinster.be/web-specific-art)
{% endcapture %}

<div class="notice">{{ notice-2 | markdownify }}</div>
