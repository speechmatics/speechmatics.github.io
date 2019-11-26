---
layout: default
title: Open Source at Speechmatics
---

<section class="hero is-medium is-dark">
  <div class="hero-body">
    <div class="container">
      <p class="title is-1">
        Speechmatics ❤  Open Source
      </p>
    </div>
  </div>
</section>

<section class="section">
  <div class="container">
    <div class="tile is-ancestor">

{% for repo in site.data.repos %}
      <div class="tile is-parent is-4">
        <article class="tile is-child notification">
          <p class="title">
            {{ repo.name }}
            <span class="icon is-medium is-pulled-right"><i class="devicon-{{ repo.language }}-plain"></i></span>
          </p>
          <p class="subtitle">{{ repo.description }}</p>
          <a class="button" href="https://github.com/speechmatics/{{ repo.name }}">GitHub</a>
        </article>
      </div>
{% endfor %}

    </div>
  </div>
</section>

<footer class="footer">
  <div class="container">
    <div class="content is-size-7">
      <div class="has-text-left">
        &copy; 2019 Cantab Research Ltd.
        <div class="is-pulled-right">
        Last Updated: {{ site.time }}
        </div>
      </div>
    </div>
  </div>
</footer>
