---
title: Publications
layout: page
permalink: /publications.html
class: publications
hide-title: true
---

# Under Review

{% bibliography --query @*[note=(under review)] %}

# Publications

{% bibliography --query @*[note!=(under review)] %}
