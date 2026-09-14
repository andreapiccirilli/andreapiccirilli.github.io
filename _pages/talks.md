---
title: "Talks"
layout: page
permalink: /talks/
---

# Talks

{% if site.data.talks %}
{% for talk in site.data.talks %}
{% include talk.html talk=talk %}
{% endfor %}
{% else %}

<p>No talks listed yet.</p>
{% endif %}
