---
title: Team
nav:
  order: 3
  tooltip: About our team
---
## Principal Investigator

{% capture left %}
  {% include portrait.html lookup="jungbeom-lee" width=400 %}
{% endcapture %}

{% capture right %}
**Jungbeom Lee**  
Assistant Professor, Korea University  
Email: your.email@korea.ac.kr  
[Google Scholar](/) · [GitHub](/)

- Research interests: Data-centric AI, Vision, Generative AI  
- Past: Amazon Applied Scientist, etc.
{% endcapture %}

{%
  include cols.html
  col1=left
  col2=right
%}

---

## PhD Students

{%
  include list.html
  data="members"
  component="portrait"
  filter="role == 'phd' and !alumni"
  style="tiny"
%}
