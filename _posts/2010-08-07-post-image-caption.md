---
layout: post
title: "Post: Image (Caption)"
categories:
  - Post Formats
tags:
  - image
  - Post Formats
---

{% capture fig_img %}
![Foo](https://raw.githubusercontent.com/daoyking/daoyking.github.io/master/images/unsplash-gallery-image-3.jpg)
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Photo from Unsplash.</figcaption>
</figure>
