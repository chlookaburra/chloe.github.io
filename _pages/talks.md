---
title: "Talks"
layout: gridlay
sitemap: false
permalink: /talks/
---

## Talks

<div class="section-card" id="pubList">
<h3>Invited Lectures and Workshops</h3>

{% bibliography --query @incollection[keywords ^= invited] %}

<h3>Conferences</h3>

{% bibliography --query @incollection[keywords != invited] %}
</div>
