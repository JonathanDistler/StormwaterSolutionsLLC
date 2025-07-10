---
layout: default
title: Projects
permalink: /projects/
---

<div class="section-title" data-aos="fade-right">Projects</div>
<div class="row">
  {% for project in site.projects %}
  <div class="col-md-6 col-lg-4 mb-4" data-aos="fade-up">
    <div class="card project-card h-100 shadow-sm">
      <div class="card-body">
        <h5 class="card-title text-primary">{{ project.title }}</h5>
        <p class="card-text">{{ project.excerpt | markdownify | strip_html | truncate: 120 }}</p>
        <a href="{{ project.url | relative_url }}" class="btn btn-primary mt-2">Read More</a>
      </div>
    </div>
  </div>
  {% endfor %}
</div>
