---
title: "Publications"
layout: gridlay
sitemap: false
permalink: /publications/
---

## Publications

<input type="text" class="pub-search" id="pubSearch" placeholder="Filter by title, author, or year...">

<div class="section-card" id="pubList">

<h3>Journal Publications</h3>

{% bibliography --query @article %}

<h3>Book Chapters</h3>

{% bibliography --query @incollection %}

</div>
