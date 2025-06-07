---
layout: page
title: Projects
icon: fas fa-project-diagram
order: 3
---
<div id="post-list" class="flex-grow-1 px-xl-1">
  {% assign projects = site.projects | sort: 'date' | reverse %}
  {% for project in projects %}
  <article class="card-wrapper card">
    <a href="{{ project.url | relative_url }}" class="post-preview row g-0 flex-md-row-reverse">
      <div class="col-md-5">
        {% if project.image %}
        <div class="preview-img">
          <img data-src="{{ project.image | relative_url }}" alt="{{ project.title }}" data-lqip="true" class="lazyload">
        </div>
        {% endif %}
      </div>
      <div class="col-md-7">
        <div class="card-body d-flex flex-column">
          <h1 class="card-title my-2 mt-md-0">{{ project.title }}</h1>
          <div class="card-text content mt-0 mb-3">
            <p>{{ project.excerpt }}</p>
          </div>
          <div class="post-meta flex-grow-1 d-flex align-items-end">
            <div class="me-auto">
              {% if project.date %}
              <i class="far fa-calendar fa-fw me-1"></i>
              <time data-ts="{{ project.date | date: '%s' }}" data-df="ll">
                {{ project.date | date: '%b %-d, %Y' }}
              </time>
              {% endif %}
              {% if project.categories %}
              <i class="far fa-folder-open fa-fw ms-3 me-1"></i>
              <span class="categories">
                {{ project.categories | join: ", " }}
              </span>
              {% endif %}
            </div>
          </div>
        </div>
      </div>
    </a>
  </article>
  {% endfor %}
</div>

