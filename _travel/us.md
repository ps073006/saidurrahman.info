---
title: "US States"
excerpt: "Visited US State with images <br/><img src='/images/us.png'>"
collection: Travel
---
{% for post in site.states %}
    <img src={{post.image}} style="width:100%">
{% endfor %}
