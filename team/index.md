---
title: Team
nav:
  order: 3
  tooltip: About our team
---

## Principal Investigator

{% capture col_left %}
  {%
    include portrait.html
    lookup="jungbeom-lee"   # 파일명에서 .md 뺀 값
    style="small"
  %}
{% endcapture %}

{% capture col_right %}
**Jungbeom Lee**  
Assistant Professor, Korea University  
Email: your.email@korea.ac.kr  
[Google Scholar](/) · [GitHub](/)

- Research interests: Data-centric AI, Vision, Generative AI  
- Past: Amazon Applied Scientist, etc.
{% endcapture %}

{%
  include cols.html
  col1=col_left
  col2=col_right
%}

---

## PhD Students

{% comment %}
아래: PhD 학생을 2열로 나누어 나열
- 템플릿의 'list'로 members를 role=phd로 필터
- 두 컬럼으로 나누기 위해 Liquid로 짝/홀 인덱스를 분리
- 각 항목은 portrait 컴포넌트의 'tiny' 스타일 + 옆에 정보


{% assign phd_all = site.members | where:"role","phd" %}

{% capture left_col %}
  {% for m in phd_all %}
    {% if forloop.index0 | modulo: 2 == 0 %}
      {% capture row_left %}
        {%
          include portrait.html
          lookup=m.slug
          style="tiny"
        %}
        **{{ m.name }}**  
        Email: {{ m.links.email }}  
        Interests: {{ m.interests }}
      {% endcapture %}
      {%
        include card.html
        title=""
        description=row_left
        style="small"
      %}
    {% endif %}
  {% endfor %}
{% endcapture %}

{% capture right_col %}
  {% for m in phd_all %}
    {% if forloop.index0 | modulo: 2 == 1 %}
      {% capture row_right %}
        {%
          include portrait.html
          lookup=m.slug
          style="tiny"
        %}
        **{{ m.name }}**  
        Email: {{ m.links.email }}  
        Interests: {{ m.interests }}
      {% endcapture %}
      {%
        include card.html
        title=""
        description=row_right
        style="small"
      %}
    {% endif %}
  {% endfor %}
{% endcapture %}

{%
  include cols.html
  col1=left_col
  col2=right_col
%}




{% endcapture %}
{% endcomment %}
{% include grid.html style="square" content=content %}
