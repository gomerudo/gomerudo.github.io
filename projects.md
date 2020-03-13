---
layout: page
permalink: /projects/
title: projects
# description: A list of my favorite personal projects.
---

# Research
<hr>

<!-- Research projects -->
<ul class="post-list">
{% for project in site.projects reversed %}
    {% if project.type == "research" %}
        <li>
            <h2><a class="poem-title" href="{{ project.purl }}" target="_blank">{{ project.title }}</a></h2>
            <!-- <p class="post-meta">{{ project.date | date: '%B %-d, %Y — %H:%M' }}</p> -->
            <p class="post-meta">({{ project.year }}) {{ project.description }}</p>
        </li>
    {% endif %}
{% endfor %}
</ul>

# Open Source
<hr>

<!-- Software projects -->
<ul class="post-list">
{% for project in site.projects reversed %}
    {% if project.type == "software" %}
        <li>
            <h2><a class="poem-title" href="{{ project.purl }}" target="_blank">{{ project.title }}</a></h2>
            <!-- <p class="post-meta">{{ project.date | date: '%B %-d, %Y — %H:%M' }}</p> -->
            <p class="post-meta">({{ project.year }}) {{ project.description }}</p>
        </li>
    {% endif %}
{% endfor %}
</ul>

