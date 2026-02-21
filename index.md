---
layout: home
title: The Compendium
---

<div class="home-page">

  <div class="hero">
    <h1>StudyBase</h1>
    <p>A specialized repository of techniques, strategies, and notes across various academic subjects.</p>
  </div>

  <div class="wrapper">

    <h2>Explore Subjects</h2>

    <div class="topic-list">
      {% for subject in site.data.subjects %}
        <div class="topic-item">
          <h3><a href="{{ subject.url | relative_url }}">{{ subject.title }}</a></h3>
          <p>{{ subject.description }}</p>
          <div class="read-time">{{ subject.meta }}</div>
        </div>
      {% endfor %}
    </div>

    <h2>Participation</h2>

    <p>The Compendium is a community-driven project. Whether you're an expert in Mathematics, a Lead Developer, or a History scholar, you can contribute your knowledge.</p>

    <p><a href="{{ '/about/' | relative_url }}" class="contribute-link">Learn how to contribute &rarr;</a></p>

  </div>

</div>
