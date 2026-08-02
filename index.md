---
layout: splash
author_profile: true
title: "Sandra Fauconnier"
excerpt: "Projects since the 1990s, at the intersection of cultural heritage and digital technology."
feature_row:
  - image_path: /assets/images/carshare.gif
    alt: "Freelance work"
    title: "Freelance work"
    excerpt: "Overview of freelance projects."
    url: /projects/freelance/
    btn_label: "Read More"
    btn_class: "btn--primary"
  - image_path: /assets/images/wikiflix-lgbtq-directors.jpg
    alt: "WikiFlix"
    title: "WikiFlix"
    excerpt: "An experimental public domain film browser, based on Wikidata."
    url: /projects/wikiflix/
    btn_label: "Read More"
    btn_class: "btn--primary"
  - image_path: /assets/images/carshare.gif
    alt: "Digital Canon of the Netherlands"
    title: "Digital Canon of the Netherlands"
    excerpt: "Mapping early digital and new media art in the Netherlands."
    url: /projects/digital-canon/
    btn_label: "Read More"
    btn_class: "btn--primary"
  - image_path: /assets/images/We_Can_Edit.jpg
    alt: "Wikimedia contributions"
    title: "Wikimedia contributions"
    excerpt: "I actively contribute to commons-based projects, like Wikipedia, Wikidata, Wikimedia Commons, OpenStreetMap."
    url: /projects/wikimedia/
    btn_label: "Read More"
    btn_class: "btn--primary"
---

## Featured projects

{% include feature_row %}

[View all projects]({{ site.baseurl }}/projects/){: .btn .btn--inverse}

## Recent posts

<ul>
{% for post in site.posts limit:5 %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="page__date">{{ post.date | date: "%-d %B %Y" }}</span>
  </li>
{% endfor %}
</ul>

[View the blog]({{ site.baseurl }}/blog/){: .btn .btn--inverse}

## Tags

{% assign all_content = site.posts | concat: site.projects %}
{% assign tags_list = "" %}
{% for item in all_content %}
  {% for tag in item.tags %}
    {% assign tags_list = tags_list | append: tag | append: "," %}
  {% endfor %}
{% endfor %}
{% assign tags_list = tags_list | split: "," | uniq | sort %}

<p class="page__taxonomy">
{% for tag in tags_list %}<a href="{{ site.tag_archive.path }}#{{ tag | slugify }}" class="page__taxonomy-item">{{ tag }}</a>{% unless forloop.last %}<span class="sep">, </span>{% endunless %}{% endfor %}
</p>
