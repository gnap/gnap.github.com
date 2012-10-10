---
layout: page
title: "GNAP's Not Another Programmer!"
tagline: Supporting tagline
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts limit:10 %}
    <li><h3><a class="tit" href="{{ BASE_PATH }}{{ post.url }}" target="_blank">{{ post.title }}</a></h3> -- <span class="post-sub">{{ post.date | date_to_string }}</span>
        <p class="abstract"><a href="{{ BASE_PATH }}{{ post.url }}"  target="_blank" title="Read more...">{{ post.content | strip_html | truncatewords:50 }}</a></p>
    </li>
  {% endfor %}
</ul>

