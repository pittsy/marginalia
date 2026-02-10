---
layout: default
title: Marginalia
---

<h1>{{ page.title }}</h1>

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-date">{{ post.date | date: "%B %-d, %Y" }}</span>
      <h2>
        <a href="{{ site.baseurl }}{{ post.url }}">
          {{ post.title }}
        </a>
      </h2>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
