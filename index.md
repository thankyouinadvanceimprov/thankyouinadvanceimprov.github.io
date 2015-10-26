---
layout: default
---
<!--
<div class="header-bar">
  <h1>TYIA</h1>
  <h2></h2>
  <br/>
  <hr>
  <br/>
</div>
-->
<div class="logo-thing" align="center">
  <img src="/img/logo.png" width="650" />
</div>

{% for project in site.portfolio %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}" />
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
        <a href="#">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}" />
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

<p>Thank You In Advance (TYIA) is an improvisational acting troupe performing in Atlanta. Our show features classic games and new creations, every show is as unique as the members of the gang.</p>

<p>You can expect a variety of games, puzzles, scenes, and sketches all based on audience suggestion and participation. We are available for everything from entertainment to variety shows. Whether it be a private or public performance, we want to make you laugh. If you want to get in touch with us, look at our <a href="about/"><u>about</u></a> page.</p>
