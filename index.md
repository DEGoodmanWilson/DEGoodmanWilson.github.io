---
layout: default
title: D.E. Goodman-Wilson
---

<div class="container">
    <div class="row">
        <div class="col-md-6 col-md-offset-3">
            <p class="lead">I’m a philosopher-engineer experienced in architecting amazing products with successful early-stage startups.</p>
            <p class="lead">My heart lies in engineering cool products with smart, friendly people. I work on Slack’s
            Platform, leading a brilliant team that builds relationships and tools with our developers. Throughout my
            career I have engaged emerging technologies from many approaches: streaming media, embedded hardware,
            TODO and even the model railroading industry. I’ve proven my grit by achieving my PhD philosophy, and my
            training in the philosophy of mind and neuroscience informs my work as an engineer.
            When I am not working, I love traveling, sailing, foreign languages and
            enjoying all life has to offer with my wife and daughter by my side.</p>
            <p>Skills yadda yadda</p>
        </div>
    </div>
    
<!-- Professional work -->
    <div class="row">
        <div class="col-md-6 col-md-offset-3">
            <h2>Professional Work</h2>
            {% assign sorted_professional = site.professional | sort:"order" %}
            {% for item in sorted_professional %}
              <h3>{{ item.title }}</h3>
              <p>{{ item.content }}</p>
            {% endfor %}
        </div>
    </div>
    
<!-- Side projects -->
    <div class="row">
        <div class="col-md-6 col-md-offset-3">
            <h2>Side Projects</h2>
            {% assign sorted_side = site.side | sort:"order" %}
            {% for item in sorted_side %}
              <h3>{{ item.title }}  <small><a href="{{ item.link }}">link</a></small></h3>
              <p>{{ item.content }}</p>
            {% endfor %}
        </div>
    </div>
    
<!-- Talks -->
    <div class="row">
        <div class="col-md-6 col-md-offset-3">
            <h2>Selected Talks</h2>
            {% assign sorted_talks = site.talks | sort:"order" %}
            {% for item in sorted_talks %}
              <h3>{{ item.title }}{% if item.link %} <small><a href="{{ item.link }}">link</a></small>{% endif %}</h3>
              {% if item.media %}
              <div class="embed-responsive embed-responsive-16by9">
                <iframe class="embed-responsive-item" src="{{ item.media }}" allowfullscreen></iframe>
              </div>
              {% endif %}
              <p>{{ item.content }}</p>
            {% endfor %}
        </div>
    </div>
</div>
