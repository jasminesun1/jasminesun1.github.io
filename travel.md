---
layout: default
title: Travel
---

<div class="travel-archive">
  
  <div class="regions-grid">
    <div class="region">
      <h1>AMERICAS</h1>
      <ul>
        {% for travel in site.travels %}
          {% if travel.region == "America" %}
            <li><a href="{{ travel.url | relative_url }}">{{ travel.location }}</a></li>
          {% endif %}
        {% endfor %}
      </ul>
    </div>

    <div class="region">
      <h1>EUROPE</h1>
      <ul>
        {% for travel in site.travels %}
          {% if travel.region == "Europe" %}
            <li><a href="{{ travel.url | relative_url }}">{{ travel.title }}</a></li>
          {% endif %}
        {% endfor %}
      </ul>
    </div>
  </div>
</div>