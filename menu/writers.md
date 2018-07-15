---
layout: page
title: Writers
---

<ul class="writers">
  {% for writer in site.writers %}

    <li itemscope>
    	<a href="{{ site.url }}/writers/{{ writer | url_param_escape }}.html"> {{ writer }} </a>
    </li>

  {% endfor %}
</ul>
