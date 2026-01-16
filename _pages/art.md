---
layout: page
title: My artistic creations ;))
permalink: /art/
collection: art
---

> In my free time, I enjoy creating small personal projects.

# Sticker sets
I’ve made several sticker sets inspired by my love for birds.  

In March 2022, I designed a sticker set based on my bird Xiao-huang (Yellow), and in Dec 2025, I made a new set featuring wood pigeons, simply because I love them. 

As of Jan 2026, the Yellow sticker set has been downloaded 1,213 times and sent 38,860 times & the pigeon set has 63 downloads and 659 sends so far. Thanks to all the bird appreciators out there! 🐦

All stickers are currently available only on the WeChat sticker gallery, but you can preview them in the sections below.  

*Feel free to use them!*

<div class="projects">

{% assign sorted_projects = site.art | sort: "importance" %}

{% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
{% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
{% endif %}

</div>
