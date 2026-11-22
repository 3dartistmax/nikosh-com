---
layout: archive
title: "Recent writings"
---

This is the personal website of Nikosh Chaulagain, featuring writing and creative work.

{% if site.posts.size == 0 %}
No writings have been published yet. Visit the [writings archive]({{ "/writings/" | relative_url }}) to check again.
{% else %}
<div class="entries-list">
  {% for post in site.posts limit:5 %}
    {% include archive-single.html type="list" %}
  {% endfor %}
</div>
{% endif %}

Explore the [gallery]({{ "/artworks/" | relative_url }}) and [status updates]({{ "/status/" | relative_url }}),
or visit the [about page]({{ "/about/" | relative_url }}).
