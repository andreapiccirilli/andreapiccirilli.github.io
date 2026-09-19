---
title: "Blog"
layout: page
permalink: /blog/
---

# Blog

Welcome to the blog section of my website! Here I plan to discuss interesting mathematics and phyiscs, which may or may not be related to my research. 
I would also like to have some introductive posts, where I'll try to make some concepts of my research as accessible as possible to non-mathematicians. 

I am doing this in my free time, therefore I don't expect to have any kind of regularity with new posts. 


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
