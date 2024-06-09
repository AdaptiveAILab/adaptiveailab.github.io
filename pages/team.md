---
layout: default
title: Team
level: 1
order: 3
description:
permalink: /team/
---

# Staff

{% assign staff = site.pages | where_exp: "item" , "item.path contains 'team/staff'"%}
{% for item in staff %}
<div class="item_wrap">
<div class="first">
    {% if item.photo and item.photo != "" %}
    <img src="{{item.photo}}" width="100px">
    {% else %}
    <img src="{% link assets/images/person.jpg %}" width="100px">
    {% endif %}    
</div>
<div class="second">
{% if item.permalink and item.permalink != "" %}
<h2><a href="{{item.permalink}}">{{item.title}}</a></h2>
{% else %}
<h2>{{item.title}}</h2>
{% endif %}    
<h3>{{item.role}}</h3>
<p>{{item.description}}</p>
</div>

</div>    
{% endfor %}

# Students

{% assign staff = site.pages | where_exp: "item" , "item.path contains 'team/students'"%}
{% for item in staff %}
<div class="item_wrap">
<div class="first">
    {% if item.photo and item.photo != "" %}
    <img src="{{item.photo}}" width="100px">
    {% else %}
    <img src="{% link assets/images/person.jpg %}" width="100px">
    {% endif %}
</div>
<div class="second">
{% if item.permalink and item.permalink != "" %}
<h2><a href="{{item.permalink}}">{{item.title}}</a></h2>
{% else %}
<h2>{{item.title}}</h2>
{% endif %}    
<h3>{{item.role}}</h3>
<p>{{item.description}}</p>
</div>

</div>    
{% endfor %}