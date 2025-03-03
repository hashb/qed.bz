---
layout: default
title: QED | URL Shortener
---

<div class="home">
  <h1 class="page-heading">Available Shortened URLs</h1>
  
  <ul class="url-list">
    {% for redirect in site.redirects %}
      <li>
        <a href="{{ site.url }}{{ site.baseurl }}/{{ redirect.path | split: '/' | last | split: '.' | first }}">
          {{ site.url }}{{ site.baseurl }}/{{ redirect.path | split: '/' | last | split: '.' | first }}
        </a>
        →
        <a href="{{ redirect.redirect_url }}" target="_blank" rel="noopener noreferrer">
          {{ redirect.redirect_url }}
        </a>
      </li>
    {% endfor %}
  </ul>
</div>
