---
layout: page
title: Mathematics
permalink: /subjects/math/
description: Techniques, strategies, and problem-solving patterns for competitive mathematics.
---

<div class="wrapper">

{% assign math_pages = site.pages | where_exp: "page", "page.path contains 'subjects/math/'" | where_exp: "page", "page.name == 'index.md'" | where_exp: "page", "page.url != '/subjects/math/'" %}

{% include topic-list.html pages=math_pages %}

</div>