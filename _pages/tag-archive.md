---
title: "Posts by Tag"
permalink: /tags/
layout: archive
author_profile: true
---

{% assign all_content = site.posts | concat: site.projects %}
{% assign tags_list = "" %}
{% for item in all_content %}
  {% for tag in item.tags %}
    {% assign tags_list = tags_list | append: tag | append: "," %}
  {% endfor %}
{% endfor %}
{% assign tags_list = tags_list | split: "," | uniq | sort %}

<ul class="taxonomy__index">
  {% for tag in tags_list %}
    {% assign tag_items = all_content | where_exp: "item", "item.tags contains tag" %}
    <li>
      <a href="#{{ tag | slugify }}">
        <strong>{{ tag }}</strong> <span class="taxonomy__count">{{ tag_items.size }}</span>
      </a>
    </li>
  {% endfor %}
</ul>

{% for tag in tags_list %}
  {% assign tag_items = all_content | where_exp: "item", "item.tags contains tag" %}
  <section id="{{ tag | slugify }}" class="taxonomy__section">
    <h2 class="archive__subtitle">{{ tag }}</h2>
    <div class="entries-list">
      {% for post in tag_items %}
        {% include archive-single.html type="list" %}
      {% endfor %}
    </div>
    <a href="#page-title" class="back-to-top">Back to Top &uarr;</a>
  </section>
{% endfor %}
