---
title: "About me"
permalink: /about me/
layout: single
---

{% for author in site.data.authors %}
{% assign member = author[1] %}
{% if member.member %}
{% if member.current %}

## {{ member.name }}

{% if member.avatar %}
![Photograph of {{member.name}}]({{member.avatar}}){:style="float: left; object-fit: contain; width: 30%; max-height: 12em; margin-left: 1em; margin-right: 1em;"}
{% endif %}

{% if member.bio %}
**{{ member.bio }}**
{% endif %}

{% if member.email %}
Email: [{{ member.email }}](mailto:{{ member.email }})
{% endif %}

{% if member.website %}
[Personal website]({{ member.website }})
{% endif %}

{% if member.twitter %}
Twitter: [@{{ member.twitter }}](https://twitter.com/{{ member.twitter }})
{% endif %}

{% if member.gscholar %}
[Google Scholar]({{ member.gscholar }})
{% endif %}

{{ member.fullbio }}

{% endif %}
{% endif %}
{% endfor %}




<!-- Former members


{% for author in site.data.authors %}
{% assign member = author[1] %}
{% if member.member %}
{% unless member.current %} -->

<!-- ### {{ member.name }}

{% if member.bio %}
**{{ member.bio }}** {% if member.start %}({{ member.start}}{% if member.end %}&ndash;{{ member.end }}{% endif %}){% endif %}
{% endif %}
{% if member.next %}
Next: {{ member.next }}
{% endif %}
{% endunless %}
{% endif %}
{% endfor %} -->

<h2>Skills:</h2>

<div class="skill-grid justified">
  <strong>Programming Languages:</strong>
  <span>Fortran, MATLAB, Python, C++, Linux/Unix, Git/GitHub, OpenMP, MPI</span><br>
  <strong>Scientific & ML Libraries:</strong>
  <span>NumPy, Scikit-learn, PyTorch</span><br>
  <strong>CFD Software:</strong>
  <span>OpenFOAM, ANSYS Fluent, ANSYS CFX, ANSYS TurboGrid</span><br>
  <strong>Visualization & Debugging:</strong>
  <span>VisIt, ParaView, Tecplot, TotalView, OriginLab</span><br>
  <strong>Meshing Software:</strong>
  <span>ICEM CFD, Rhinoceros 3D</span><br>
  <strong>Documentation:</strong>
  <span>LaTeX, Microsoft Word, Microsoft PowerPoint</span><br>
</div>

<h2>Professional Memberships:</h2>

<div class="justified">
  <ul>
    <li><strong>American Society of Mechanical Engineers (ASME)</strong> - 2019-2024</li>
    <li><strong>American Physical Society (APS)</strong> - <2023–2025</li>
    <li><strong>American Institute of Aeronautics and Astronautics (AIAA)</strong> - 2024</li>
  </ul>
</div>

<h2>Collaborations:</h2>

<div class="justified">
  <p>
    I am open to research collaborations in fluid mechanics, computational and experimental
    flow physics, data-driven modeling, and bio-inspired locomotion. My research focuses on
    force diagnostics, vorticity-based analysis, and physics-informed data-driven techniques
    to understand complex unsteady and turbulent flows in engineered and biological systems.
  </p>
</div>
