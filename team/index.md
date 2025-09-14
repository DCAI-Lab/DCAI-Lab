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
<div style="line-height:1; margin:0;">
  <p><strong>Jungbeom Lee</strong><br>
  Assistant Professor, CSE, Korea University</p>

  <p><strong>Education</strong></p>
  <ul style="margin:0; line-height:1;">
    <li>Ph.D. in ECE, Seoul National University, 2017–2023</li>
    <li>B.S. in ECE, Seoul National University, 2013–2017</li>
  </ul>

  <p><strong>Experience</strong></p>
  <ul style="margin:0; line-height:1;">
    <li>Applied Scientist, Amazon, Seattle, USA, 2023–2025</li>
    <li>Visiting Researcher, Naver AI Lab, Seongnam, Korea, 2023</li>
    <li>Applied Scientist Intern, Amazon, Seattle, USA, 2022</li>
    <li>Research Intern, Naver AI Lab, Seongnam, Korea, 2021, 2022</li>
  </ul>
</div>
{% endcapture %}

{%
  include cols.html
  col1=left
  col2=right
%}



## PhD Students

{%
  include list.html
  data="members"
  component="portrait"
  filter="role == 'phd' and !alumni"
  style="tiny"
%}
