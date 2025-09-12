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
<div style="line-height:1.3; margin-top:0.2em; margin-bottom:0.2em;">
**Jungbeom Lee**  
Assistant Professor, Korea University  

**Education**
- Ph.D. in ECE, Seoul National University, 2017-2023
- B.S. in Electrical and Computer Engineering, Seoul National University, 2013-2017

**Experience**
- Applied Scientist, Amazon, Seattle, USA 2023-2025
- Visiting Researcher, Naver AI Lab, Seongnam, Korea 2023
- Applied Scientist Intern, Amazon, Seattle, USA 2022
</div>
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
