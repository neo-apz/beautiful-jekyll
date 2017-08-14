---
layout: page
title: Parsa at EPFL
subtitle: Parallel Systems Architecture Lab
use-site-title: true
---

## Mission

Information technology has undergone a major paradigm shift with sensors,
embedded and mobile devices generating massive amounts of data
to be augmented with backend cloud services for enhanced experience.
Data has emerged as a currency for modern society.
Datacenters are now the backbone of IT offering large-scale cloud services
at low costs benefiting from and exploiting the economies of scale.
With silicon efficiency scaling having dwindled since 2004
and silicon density scaling slowing down,
future digital platforms will rely on heterogeneous logic and memory
to allow for IT scalability.

Meanwhile, the demand for large-scale cloud services has grown dramatically
faster than conventional silicon scaling making IT platform scalability
a grand challenge.
Future platforms will need hand-in-hand collaboration of application domain experts
and platform designers to improve scalability.
With many online services being in-memory and the minimum communication latency
between the farthest nodes in a 20MW datacenter being microseconds,
future server platforms will go through revolutionary changes in architecture
to enable seamless aggregation of logic and memory resources across nodes,
breaking the conventional system abstraction layers.
PARSA at EPFL engages in research and educational activities
to pioneer future server design.

<div class="posts-list">
  {% for post in paginator.posts %}
  <article class="post-preview">
    <a href="{{ post.url | prepend: site.baseurl }}">
	  <h2 class="post-title">{{ post.title }}</h2>

	  {% if post.subtitle %}
	  <h3 class="post-subtitle">
	    {{ post.subtitle }}
	  </h3>
	  {% endif %}
    </a>

    <p class="post-meta">
      Posted on {{ post.date | date: "%B %-d, %Y" }}
    </p>

    <div class="post-entry-container">
      {% if post.image %}
      <div class="post-image">
        <a href="{{ post.url | prepend: site.baseurl }}">
          <img src="{{ post.image }}">
        </a>
      </div>
      {% endif %}
      <div class="post-entry">
        {{ post.excerpt | strip_html | xml_escape | truncatewords: site.excerpt_length }}
        {% assign excerpt_word_count = post.excerpt | number_of_words %}
        {% if post.content != post.excerpt or excerpt_word_count > site.excerpt_length %}
          <a href="{{ post.url | prepend: site.baseurl }}" class="post-read-more">[Read&nbsp;More]</a>
        {% endif %}
      </div>
    </div>

    {% if post.tags.size > 0 %}
    <div class="blog-tags">
      Tags:
      {% if site.link-tags %}
      {% for tag in post.tags %}
      <a href="{{ site.baseurl }}/tag/{{ tag }}">{{ tag }}</a>
      {% endfor %}
      {% else %}
        {{ post.tags | join: ", " }}
      {% endif %}
    </div>
    {% endif %}

   </article>
  {% endfor %}
</div>

{% if paginator.total_pages > 1 %}
<ul class="pager main-pager">
  {% if paginator.previous_page %}
  <li class="previous">
    <a href="{{ paginator.previous_page_path | prepend: site.baseurl | replace: '//', '/' }}">&larr; Newer Posts</a>
  </li>
  {% endif %}
  {% if paginator.next_page %}
  <li class="next">
    <a href="{{ paginator.next_page_path | prepend: site.baseurl | replace: '//', '/' }}">Older Posts &rarr;</a>
  </li>
  {% endif %}
</ul>
{% endif %}
