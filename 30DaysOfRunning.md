---
layout: page
title: Running
permalink: /30DaysOfRunning/
---

<div class="home">

  <h1 class="page-heading">Days</h1>

  <ul class="post-list">
    {% for post in site.posts %}
      {% if post.categories contains 'running' and post.categories contains '30days' %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title | escape }}</a>
        </h2>
        <p>
        {{post.content}}
        </p>
      </li>
      {% endif %}
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div>