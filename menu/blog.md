---
layout: page
title: Blog
---
<ul class="posts">
  {% for post in site.posts %}

    <li itemscope>
      <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
      <p>
      {{ post.content | strip_html | truncate: 100 }}</p>
      <p class="post-date"><span><i class="fa fa-calendar" aria-hidden="true"></i> {{ post.date | date: "%B %-d, %Y" }} - <a href="{{ site.url }}/writers/{{ post.author | url_param_escape }}.html"> {{ post.author }} </a> - <i class="fa fa-clock-o" aria-hidden="true"></i> {% include read-time.html %}</span></p>
    </li>

  {% endfor %}
</ul>
