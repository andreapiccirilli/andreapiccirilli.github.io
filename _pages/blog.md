---
title: "Blog"
layout: page
permalink: /blog/
---

# Blog




{% if site.posts.size > 0 %}
<div class="section-card" markdown="0">
{% for post in site.posts %}
<div class="news-item" style="padding: 1rem 0; border-bottom: 1px solid var(--border-color);">
<span class="news-date">{{ post.date | date: "%b %-d, %Y" }}</span><br>
<a href="{{ post.url | relative_url }}" style="font-weight: 600;">{{ post.title }}</a>
</div>
{% endfor %}
</div>
{% else %}
<p class="text-muted">No blog posts yet.</p>
{% endif %}

From the viewpoint of topological strings, however, they are not unrelated constructions.

Closed worldsheets lead to closed-string invariants and Gromov–Witten theory. Worldsheets with boundary lead to Lagrangian boundary conditions and Floer theory. Polygons encode interactions of open strings, and organizing all possible boundary conditions naturally leads to a category.

The physics does not replace the mathematics — making any of these statements precise requires substantial work — but it provides a remarkably coherent picture of why these structures should exist in the first place.

And mirror symmetry goes one step further: it tells us that the symplectic geometry encoded by the A-model should have an entirely different description in terms of the complex and algebraic geometry of another Calabi–Yau manifold.

That is a rather extraordinary amount of geometry to come from studying the ways a string can sweep out a surface.
