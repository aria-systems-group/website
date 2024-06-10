---
title: People 
layout: page 
permalink: /people/all.html
class: people
---

{% assign sorted = site.people | sort: 'ordering' %}
{% assign sorted_alumni_ascending = site.people | sort: 'year-graduated' %}
{% assign sorted_alumni = sorted_alumni_ascending | reverse %}

{% for people in sorted %}
{% if people.status == "current" %}
<div class="flex-container">
<div class="flex-child disappearing">
{% if people.picture-link != blank %}
<a href="{{ people.picture-link }}" target="_blank"><img src="{{ site.baseurl }}{{ people.picture }}" alt="{{ people.name }}" title="{{ people.name }}"></a>
{% elsif people.generate-extra-page %}
<a href="{{ site.baseurl }}{{ people.url }}" target="_blank"><img src="{{ site.baseurl }}{{ people.picture }}" alt="{{ people.name }}" title="{{ people.name }}"></a>
{% else %}
<img src="{{ site.baseurl }}{{ people.picture }}" alt="{{ people.name }}" title="{{ people.name }}">
{% endif %}
</div>
<div class="flex-child">
<h3>
{% if people.picture-link != blank %}
<a href="{{ people.header-link }}" target="_blank">{{ people.name }}</a>
{% elsif people.generate-extra-page %}
<a href="{{ site.baseurl }}{{ people.url }}" target="_blank">{{ people.name }}</a>
{% else %}
{{ people.name }}
{% endif %}
</h3>
<div class="flex-child">
    <p>{{ people.program }}, 
    <a href="mailto:{{ people.email }}">{{ people.email }}</a>
    {{ people.excerpt | markdownify }}</p>
</div>
</div>
</div>
{% endif %}
{% endfor %}

# Alumni
{% for people in sorted_alumni %}
{% if people.status == "alumnus" %}
<div class="">
<p>{{ people.name }} - {{ people.program }}  {{ people.year-graduated }} -  {{ people.current-position }} </p>
</div>
{% endif %}
{% endfor %}


