---
layout: page
title: portfolio
permalink: /portfolio/
order: 1
---

{% for project in site.portfolio %}
<div class="project">
    <div class="thumbnail">
        <a href="{% if project.redirect %}{{ project.redirect }}{% else %}{{ site.baseurl }}{{ project.url }}{% endif %}" target="_blank">
            <div class="image-container">
                {% if project.img %}
                <img src="{{ project.img }}" alt="{{ project.title }}" />
                {% else %}
                <div class="blankbox"></div>
                {% endif %}
            </div>
            <span>
                <h1>{{ project.title }}</h1>
                <br/>
                <p>{{ project.description }}</p>
            </span>
        </a>
    </div>
</div>
{% endfor %}

