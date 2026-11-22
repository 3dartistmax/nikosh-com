---
title: "Writings"
permalink: /writings/
layout: archive
author_profile: false
---

{% assign writings = site.posts | where_exp: "post", "post.hidden != true" %}
{% if writings.size == 0 %}
No writings have been published yet.
{% else %}
<div class="entries-list">
  {% for post in writings %}
    {% include archive-single.html type="list" %}
  {% endfor %}
</div>
{% endif %}
