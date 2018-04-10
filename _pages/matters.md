---
layout: page
title: Matters
subtitle: //
permalink: /matters/
---

<div class="posts-list">
  <!--  # for matter in paginator.matters \ -->
  {% for matter in site.matters %}  
  <article class="post-preview">
    <a href="{{ matter.url | prepend: site.baseurl }}">
	  <h2 class="post-title">{{ matter.title }}</h2>
	  {% if matter.subtitle %}
	  <h3 class="post-subtitle">
	    {{ matter.subtitle }}
	  </h3>
	  {% endif %}
    </a>

	<span class="post-meta">
    <time datetime="{{ matter.date | date: "%Y-%m-%d" }}">{{ matter.date | date: "%B %-d" }}</time>
    {% if site.read-time %} - {% include read-time.html %} read{% endif %}
	</span>

    <div class="post-entry-container">
      {% if matter.image %}
      <div class="post-image">
        <a href="{{ matter.url | prepend: site.baseurl }}">
          <img src="{{ matter.image }}">
        </a>
      </div>
      {% endif %}

    </div>

   </article>
  {% endfor %}
  
  {% if paginator.total_pages > 1 %}
<ul class="pager main-pager">
  {% if paginator.previous_page %}
  <li class="previous">
    <a href="{{ paginator.previous_page_path | prepend: site.baseurl | replace: '//', '/' }}">&larr; Newer Matter</a>
  </li>
  {% endif %}
  {% if paginator.next_page %}
  <li class="next">
    <a href="{{ paginator.next_page_path | prepend: site.baseurl | replace: '//', '/' }}">Older Matter &rarr;</a>
  </li>
  {% endif %}
</ul>
{% endif %}
</div>