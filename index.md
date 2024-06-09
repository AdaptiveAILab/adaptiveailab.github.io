---
layout: default
title: Home
level: 1
order: 0
description:
permalink: /
---

# Welcome to our lab page

We are the __Adaptive AI research group__ affiliated with the [Institut for Robotics and Cognitive Systems](https://www.rob.uni-luebeck.de/institut) at the [University of Lübeck](https://www.uni-luebeck.de) in Germany.

Meet our **[team](/team/)**.

<br>
<center><font color="#DC7633">
Please note that this page was only recently initiated and is currently under construction.
</font></center>
<br>

# About our group

We are committed to developing __autonomous AI systems__ that can __continually learn__ and __adapt__ to __dynamic environments__. We are working on __hierarchical__ and __recurrent neural architectures__, along with corresponding __biologically plausible learning methods__, to facilitate __flexible__, __efficient__, and __scalable learning__ amidst __high-throughput sensory data streams__. One of our primary objectives is to __optimize efficiency__, ensuring that these systems can __function effectively despite resource constraints__ such as limited energy supply, memory, and computational power. It is our goal to contribute to __greening AI__, complementing big data-driven learning approaches with compact, efficient, and more __sustainable solutions__. On a higher level, we aim at fostering interdisciplinary research linking machine learning, cognitive science, and robotics to drive innovative progress.

Learn more about our **[research](/research/)**.


# Latest news
<ul>
{% for post in site.posts limit:5 %}
    <li>
        [{{post.date | date: "%b %d, %Y" }}] <a href="{{post.url}}">{{post.title}}</a>
    </li>
{% endfor %}
</ul>
Find more news [here](/news/).
