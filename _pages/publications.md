---
layout: archive
title: "First-Author Publications"
permalink: /publications/
author_profile: true
---
<!-- {% include toc %} -->

{% include base_path %}

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
