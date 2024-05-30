---
layout: page
title: Photo Gallery
permalink: /gallery/
---

<div class="gallery">
  {% for image in site.static_files %}
    {% if image.path contains '/assets/img/gallery/' %}
      <div class="gallery-item">
        <a href="{{ image.path }}" target="_blank">
          <img src="{{ image.path }}" alt="{{ image.name }}">
        </a>
      </div>
    {% endif %}
  {% endfor %}
</div>
