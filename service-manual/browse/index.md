---
layout: browse
title: Browse guides by topic
subtitle: A list of all guides
category: home
status: draft
breadcrumbs:
  -
    title: Home
    url: /service-manual
---

<div class="article-container group">
  <div class="contents">
    <nav>
      <h2>Contents</h2>

      <ol>
        <li><a href="#agile">Agile</a></li>
        <li><a href="#assisted-digital">Assisted digital</a></li>
        <li><a href="#making-software">Making software</a></li>
        <li><a href="#measurement">Measurement</a></li>
        <li><a href="#operations">Operations</a></li>
        <li><a href="#phases">Phases</a></li>
        <li><a href="#identity-assurance">Identity assurance</a></li>
        <li><a href="#technology">Technology</a></li>
        <li><a href="#the-team">The team</a></li>
        <li><a href="#user-centered-design">User-centered design</a></li>
      </ol>
    </nav>
  </div>

  <div class="inner">
    <div class="link-list">
      <h2 id="agile">Agile</h2>
      {% assign link_cat = 'agile' %}
      {% include _browse-links.html %}

      <h2 id="assisted-digital">Assisted digital</h2>
      {% assign link_cat = 'assisted-digital' %}
      {% include _browse-links.html %}

      <h2 id="making-software">Making software</h2>
      {% assign link_cat = 'making-software' %}
      {% include _browse-links.html %}

      <h2 id="measurement">Measurement</h2>
      {% assign link_cat = 'measurement' %}
      {% include _browse-links.html %}

      <h2 id="operations">Operations</h2>
      {% assign link_cat = 'operations' %}
      {% include _browse-links.html %}

      <h2 id="phases">Phases</h2>
      {% assign link_cat = 'phases' %}
      {% include _browse-links.html %}

      <h2 id="identity-assurance">Identity assurance</h2>
      {% assign link_cat = 'identity-assurance' %}
      {% include _browse-links.html %}

      <h2 id="technology">Technology</h2>
      {% assign link_cat = 'technology' %}
      {% include _browse-links.html %}

      <h2 id="the-team">The team</h2>
      {% assign link_cat = 'the-team' %}
      {% include _browse-links.html %}

      <h2 id="user-centered-design">User-centered design</h2>
      {% assign link_cat = 'user-centered-design' %}
      {% include _browse-links.html %}
    </div>
  </div>
</div>
