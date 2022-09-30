---
layout: default
title:  "Blog"
---
<ul>
  {% for post in site.posts %}
  <li>
    <h2>
      <a href="{{ post.url | relative_url}}">
        {{ post.title }}
      </a>
    </h2>
    <time style="font-style: italic;" datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
  </li>
{% endfor %}
</ul>