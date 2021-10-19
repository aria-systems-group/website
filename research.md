---
title: Projects 
layout: page 
permalink: /projects/all.html
class: research
---

ARIA Systems group develops novel theoretical foundations and computational frameworks to enable reliable and intelligent autonomy. The main theme of our work is safety and soundness, and the emphasis is on safe autonomy through correct-by-construction algorithmic approaches. Our research builds on knowledge developed in control theory, formal methods, statistical reasoning, and machine learning & AI to address real-world challenges in robotics and safety-critical systems. 

# Current Projects
{% assign sorted = site.projects | sort: 'ordering'  %}
{% for projects in sorted %}
{% if projects.status == "current" %}
<div class="bottom-border">
    <h6>
    {% if projects.link-flag %}
    <a href="{{ site.baseurl }}{{ projects.url }}">{{ projects.name }}</a> 
    {% else %}
   {{ projects.name }}
    {% endif %}
    </h6>
    {{ projects.excerpt | markdownify }}
</div>
{% endif %}
{% endfor %}

# Past Work
{% assign sorted = site.projects | sort: 'ordering'  %}
{% for projects in sorted %}
{% if projects.status == "past" %}
<!-- What do sections do ?? -->
<section class=""> 
<div class="">
<!-- <div class="mbr-figure align-center" style="width: 20%;">
    <a href="" target="_blank"><img src= "{{ projects.picture }}" alt="Mobirise" title="John Jackson"></a>
</div> -->
<div class="">
    <!-- <h2 class="pt-2 mbr-fonts-style display-5"> -->
    <h6>
    {% if projects.link-flag %}
    <a href="{{ site.baseurl }}{{ projects.url }}">{{ projects.name }}</a>
    {% else %}
    {{ projects.name }} 
    {% endif %}
    </h6>
</div>
</div>
</section>
{% endif %}
{% endfor %}