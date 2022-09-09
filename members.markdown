---
layout: page
title: Members
permalink: /members/
---

<div class="grid">

{% randoms site.members members %}
{% for member in members  %}
 <a href="{{member.slug}}">
	<img src="https://github.com/{{ member.github }}.png?size=80" class="grid-img" alt="{{member.name}}" title="{{ member.name }} - {{ member.position }} @ {{member.company}}"/>
	</a>
{% endfor %}
</div>
