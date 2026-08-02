---
layout: archive
author_profile: true
title: "Sandra Fauconnier"
---

{% assign p1 = site.projects | where: "title", "Freelance work" %}
{% assign p2 = site.projects | where: "title", "WikiFlix" %}
{% assign p3 = site.projects | where: "title", "Digital Canon of the Netherlands" %}
{% assign p4 = site.projects | where: "title", "Wikimedia contributions" %}
{% assign featured = p1 | concat: p2 | concat: p3 | concat: p4 %}

## Featured projects

<div class="entries-grid">
  {% include documents-collection.html entries=featured type="grid" %}
</div>

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
