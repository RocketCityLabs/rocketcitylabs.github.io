---
layout: page
title: Blog
---
<ul class="posts">
  {% for post in site.posts %}

    <li itemscope>
      <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
      <p class="post-date"><span><i class="fa fa-calendar" aria-hidden="true"></i> {{ post.date | date: "%B %-d %Y" }} - <a href="{{ site.url }}/authors/{{ post.author }}.html">  </a> - <i class="fa fa-clock-o" aria-hidden="true"></i> {% include read-time.html %}</span></p>
    </li>

  {% endfor %}
</ul>
