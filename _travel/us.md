---
title: "US States"
excerpt: "Visited US State with images <br/><img src='/images/us.png'>"
collection: Travel
---
{% for post in site.states %}
    {{post.image}}
    <img src={{post.image}} style="width:100%">
{% endfor %}
