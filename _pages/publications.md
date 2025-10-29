---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

## Peer-Reviewed Journals

{% assign journal_papers = site.publications | where: 'type', 'journal' %}

{% for post in journal_papers reversed %}
  {% include archive-single.html %}
{% endfor %}

## International Conferences

{% assign conference_papers = site.publications | where: 'type', 'conference' %}

{% for post in conference_papers reversed %}
  {% include archive-single.html %}
{% endfor %}
