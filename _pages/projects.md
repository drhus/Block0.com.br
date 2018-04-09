---
layout: page
title: Projects
permalink: /projects/
subtitle: //
description: Projects List
---

<div class="posts-list">
    {% for project in site.projects %}
  <article class="post-preview">
    <a href="{{ project.url | prepend: site.baseurl }}">
	  <h2 class="post-title">{{ project.title }}</h2>
	  {% if project.subtitle %}
	  <h3 class="post-subtitle">
	    {{ project.subtitle }}
	  </h3>
	  {% else %}
	  <h3 class="post-subtitle">
        {{ project.excerpt | strip_html | xml_escape | truncatewords: site.excerpt_length }}
        {% assign excerpt_word_count = project.excerpt | number_of_words %}
	  </h3>	  
	  {% endif %}
    </a>
	<!-- LessIsMore
    <div class="project-entry-container">
      {% if project.image %}
      <div class="project-image">
        <a href="{{ project.url | prepend: site.baseurl }}">
          <img src="{{ project.image }}">
        </a>
      </div>
      {% endif %}
    </div>

    {% if project.tags.size > 0 %}
    <div class="blog-tags">
      Tags:
      {% if site.link-tags %}
      {% for tag in project.tags %}
      <a href="{{ site.baseurl }}/tags#{{- tag -}}">{{- tag -}}</a>
      {% endfor %}
      {% else %}
        {{ project.tags | join: ", " }}
      {% endif %}
    </div>
    {% endif %}
	//-->
   </article>
  {% endfor %}
</div>