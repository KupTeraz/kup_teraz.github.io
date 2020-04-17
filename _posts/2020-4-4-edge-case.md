---
title: Cattastophe
layout: single
permalink: /cats/kewl/
catagories: [kewl, cats]
date: 2020-4-18 17:01:00 
author-profile: true
related: true
share: true
read_time: true
---

Here is a kewl post about cats

<div class="post-categories">
  {% if post %}
    {% assign categories = post.categories %}
  {% else %}
    {% assign categories = page.categories %}
  {% endif %}
  {% for category in categories %}
  <a href="{{site.baseurl}}/categories/#{{category|slugize}}">{{category}}</a>
  {% unless forloop.last %}&nbsp;{% endunless %}
  {% endfor %}
</div>