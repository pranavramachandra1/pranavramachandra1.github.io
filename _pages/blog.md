---
layout: archive
title: "Blog"
permalink: /blog/
author_profile: true
---

{% if site.author.googlescholar %}
    <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

{% for post in site.posts reversed %}
  {% include archive-single.html %}
{% endfor %}
