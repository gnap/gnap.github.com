---
layout: page
title: "Welcome!"
tagline: "GNAP's Not Another Programmer!"
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts limit:10 %}
    <li><h3><a class="tit" href="{{ BASE_PATH }}{{ post.url }}" target="_blank">{{ post.title }}</a></h3> -- <span class="post-sub">{{ post.date | date_to_string }}</span>
        <p class="abstract">{{ post.content }}</p>
        <p><a href="{{ BASE_PATH }}{{ post.url }}"  target="_blank" title="Read more...">more...</a></p>
    </li>
  {% endfor %}
</ul>

