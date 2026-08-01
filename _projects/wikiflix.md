---
layout: single
title: "WikiFlix"
date_start: 2019-11-22
date_end: 
tags: [Wikimedia, Commons]
header:
  image: /assets/images/wikiflix-lgbtq-directors.jpg
  teaser: /assets/images/wikiflix-lgbtq-directors.jpg
excerpt: "An experimental public domain film browser, based on Wikidata"
---

{{ page.date_start | date: "%Y" }}{% if page.date_end %} – {{ page.date_end | date: "%Y" }}{% else %} – {% endif %}

I started WikiFlix as a hobby project at the Wiki Techstorm in Amsterdam, in November 2019: a Wikidata-driven mini-portal on Wikimedia Commons for browsing and watching public domain films, à la Netflix. Wikimedia Commons hosts huge amounts of freely licensed audiovisual material, but it's badly described and hard to discover. I wanted to show what structured data — and Wikidata as a backbone — could do to make that content browsable and discoverable, not just stored.

It stayed a small side project, built with basic SPARQL queries and Listeria lists, and I never developed it much further myself.

In 2024, Wikimedia developer Magnus Manske picked up the idea and built a proper version of it: a live tool hosted on Wikimedia Toolforge, streaming thousands of public-domain films sourced from Wikimedia Commons, the Internet Archive and YouTube, with its database updated hourly from Wikidata.

{% capture notice-2 %}
#### Read more

* [WikiFlix, Magnus Manske's live version](https://wikiflix.toolforge.org/)
* [My original notes on WikiFlix and dynamic multimedia portals](https://commons.wikimedia.org/wiki/User:Spinster/Thoughts_about_WikiFlix_%28and_dynamic_multimedia_portals%29)
* [Full overview of press coverage](https://www.wikidata.org/wiki/Help:WikiFlix/Press), including a small selection:
  * [TechCrunch: "WikiFlix shows us what Netflix would have been like 100 years ago"](https://techcrunch.com/2025/12/16/wikiflix-shows-us-what-netflix-would-have-been-like-100-years-ago/)
  * [Gizmodo: "WikiFlix Helps You Catch Up on Films That Just Entered the Public Domain"](https://gizmodo.com/wikiflix-helps-you-catch-up-on-films-that-just-entered-the-public-domain-2000708070)
  * [Open Culture: "Stream 4,000+ Public Domain Movies on WikiFlix"](https://www.openculture.com/2026/01/stream-4000-public-domain-movies-on-wikiflix.html)
  * [Boing Boing: "WikiFlix is like Netflix for public domain films, with no ads, no logins, and no data harvesting"](https://boingboing.net/2026/01/27/wikiflix-is-like-netflix-for-public-domain-films-with-no-ads-no-logins-and-no-data-harvesting.html)
  * [Wikipedia Signpost coverage](https://en.wikipedia.org/wiki/Wikipedia:Wikipedia_Signpost/2026-02-17/News_and_notes)
{% endcapture %}

<div class="notice">{{ notice-2 | markdownify }}</div>
