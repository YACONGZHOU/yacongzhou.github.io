
---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## Academic Positions

- **Postdoctoral Researcher**  
  Shenzhen Institutes of Advanced Technology, Chinese Academy of Sciences

## Education

- **Ph.D. in Computer Science**, 2025  
  Royal Holloway, University of London  
  Supervisors: [Gregory Gutin](https://pure.royalholloway.ac.uk/en/persons/gregory-gutin/) and Stefanie Gerke  
  Thesis: [Partition Problems for Directed and Undirected Graphs](https://pure.royalholloway.ac.uk/en/publications/partition-problems-for-directed-and-undirected-graphs/)

- **Master's Degree**  
  Shanghai University  
  Supervisor: Liying Kang

## Research Interests

Graph Theory, Extremal Combinatorics, and Theoretical Computer Science.

## Publications

{% assign sorted_publications = site.publications | sort: 'date' | reverse %}
<ul>
{% for post in sorted_publications %}
  <li>
    {% if post.link %}
      <a href="{{ post.link }}">{{ post.title }}</a>
    {% else %}
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    {% endif %}
    {% if post.venue %}, <em>{{ post.venue }}</em>{% endif %}
    {% if post.date %} ({{ post.date | date: "%Y" }}){% endif %}
    {% if post.excerpt %}
      <div><small>{{ post.excerpt }}</small></div>
    {% endif %}
  </li>
{% endfor %}
</ul>

## Talks and Presentations

{% assign sorted_talks = site.talks | sort: 'date' | reverse %}
<ul>
{% for post in sorted_talks %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    {% if post.venue %}, {{ post.venue }}{% endif %}
    {% if post.date %} ({{ post.date | date: "%B %Y" }}){% endif %}
  </li>
{% endfor %}
</ul>

## Teaching

{% assign sorted_teaching = site.teaching | sort: 'date' | reverse %}
<ul>
{% for post in sorted_teaching %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    {% if post.venue %}, {{ post.venue }}{% endif %}
    {% if post.date %} ({{ post.date | date: "%Y" }}){% endif %}
  </li>
{% endfor %}
</ul>
  

## Academic Service

**Referee for:**
- Journal of Graph Theory
- SIAM Journal on Discrete Mathematics
- The Electronic Journal of Combinatorics
- European Journal of Combinatorics
- Discrete Mathematics
