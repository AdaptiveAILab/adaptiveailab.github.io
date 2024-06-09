---
layout: default
title: News
level: 1
order: 2
description:
permalink: /news/
---

# News
<ul>
{% for post in site.posts limit:100 %}
    <li>
        [{{post.date | date: "%b %d, %Y" }}] <a href="{{post.url}}">{{post.title}}</a>
    </li>
{% endfor %}
</ul>