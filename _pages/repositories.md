---
layout: page
permalink: /repositories/
title: Research Projects
description: My research projects in public policy, data analysis, and social sciences. Each project includes code, analysis, and detailed documentation.
nav: true
nav_order: 3
---




{% if site.data.repositories.github_repos %}
### Project Details

{% for repo in site.data.repositories.github_repos %}
  {% include repository/repo_with_description.html repository=repo %}
{% endfor %}
{% endif %}



## Technical Skills

- **Statistical Analysis**: R, Julia, regression modeling, fixed effects, logistic regression
- **Data Management**: NSS, IHDS, and other socio-economic datasets
- **Research Tools**: Git version control, LaTeX documentation, reproducible research workflows
- **Policy Research**: Literature review, archival research, fieldwork, data visualization

---

