---
layout: page
title: Photo Gallery
permalink: /gallery/
---

<h2>Photography</h2>
<div class="gallery">
  {% for image in site.static_files %}
    {% if image.path contains '/assets/img/gallery/photography/' %}
      <div class="gallery-item">
        <a href="{{ image.path }}" target="_blank">
          <img src="{{ image.path }}" alt="{{ image.name }}">
        </a>
      </div>
    {% endif %}
  {% endfor %}
</div>

<h2>Art</h2>
<div class="gallery">
  {% for image in site.static_files %}
    {% if image.path contains '/assets/img/gallery/art/' %}
      <div class="gallery-item">
        <a href="{{ image.path }}" target="_blank">
          <img src="{{ image.path }}" alt="{{ image.name }}">
        </a>
      </div>
    {% endif %}
  {% endfor %}
</div>