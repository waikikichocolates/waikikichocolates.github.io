---
layout: page-fullwidth
title:  "How It Started"
teaser: "Waikiki Chocolate History"
tags:
    - Waikiki Chocolates
    - Chocolate Truffles
categories:
    - about
    - business
header: no
permalink: /about/business/ourhistory/
---
<div class="row align-center">
  <div class="columns large-10">
<div class="timeline">
{% for events in site.ourhistory %}
  <div class="timeline-item">
    <div class="timeline-icon">
      <img src="{{ site.urlimg }}/about/business/greenfavicon-32x32.png" class="" height="21" width="21" alt="">
    </div>
    <div class="timeline-content {% cycle " " , "right" %}">
      <p class="timeline-content-date">{{events.eventdate}}</p>
      <p>{{ events.content }}</p>
      <img src="{{ site.urlimg }}/about/business/ourhistory/{{ events.eventimage }}" class="" height="200" alt="">
    </div>
  </div>
{% endfor %}
</div>

  </div>
</div>



{% include list-posts tag='post format' %}
