---
layout: page
title: Members
permalink: /members/
---

{% for member in site.members %}
  <img src="https://github.com/{{ member.github }}.png?size=120" alt="{{member.name}}" title="{{ member.name }} - {{ member.position }} @ {{member.company}}"/>
  <a href="{{ member.url }}">
    {{ member.name }}
  </a>
{% endfor %}
