---
layout: page
title: About
permalink: /about/
weight: 3
---

# **About Me**

Hi, I’m **{{ site.author.name }}** :wave:, a full-stack + AI engineer focused on building scalable systems, ML pipelines, and production-quality tooling. I enjoy turning messy data and complex architectures into reliable products that ship fast and stay maintainable.

---

## Working Experience
{% include about/timeline.html title="Working Experience" source=site.data.timeline-work %}

---

## Education
{% include about/timeline.html title="Education" source=site.data.timeline-education %}

---

## Skills
<div class="row">
{% include about/skills.html title="Programming Skills" source=site.data.programming-skills %}
{% include about/skills.html title="Other Skills" source=site.data.other-skills %}
</div>