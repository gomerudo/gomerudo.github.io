---
layout: page
title: resumé
permalink: /resume/
---

For a detailed description of each of my professional and academic milestones, click the images 
below. You can also get a 
<a href="https://drive.google.com/open?id=1MW1olQMlSSkfYh6rFFbCUdrTnW2ivXWf" target="_blank">
one-page version of my CV</a>. I also encourage you to visit my <a 
href="https://github.com/gomerudo" target="_blank">Github profile</a> to check out my skills and 
work, and <a href="https://scholar.google.com/citations?user=YrHcTgIAAAAJ&hl=en" 
target="_blank">Scholar</a> for publications.

{% for project in site.resume %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}

<div class="project ">
    <div class="thumbnail">
        <a href="{{ site.baseurl }}{{ project.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endif %}

{% endfor %}

<!-- <br/>
<hr/>
<br/>
<span class="contacticon center">
	<a href="mailto:j.gomezrb.dev@gmail.com"><i class="fa fa-envelope-square"></i></a>
	<a href="https://github.com/gomerudo" target="_blank"><i class="fa fa-github-square"></i></a>
	<a href="https://www.linkedin.com/in/jgomezrb" target="_blank"><i class="fa fa-linkedin-square"></i></a>
</span>

<div class="col three caption">
	The best way to contact me is via email, but feel free to reach me through your favorite choice.
</div>
 -->
