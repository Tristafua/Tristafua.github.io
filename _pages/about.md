---
layout: single
permalink: /
title: "Homepage"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

## About Me {#about}
I'm a second year Master student from Institute of Basic Medical Sciences Chinese Academy of Medical Sciences, School of Basic Medicine Peking Union Medical College. I am very fortunate to be advised by Prof. Yamei NIU o and Prof. Wei-Ming Tong from Peking Union Medical College / Chinese Academy of Medical Sciences.
    
My research interests focus on:m6A modification, mitochondria and neurodegenerative diseases. 

I'm finding some PhD positions, so if you're interested in me, feel free to [email me](mailto:fyjjade5525@gmail.com).

## Education 🧑‍🎓 {#education}
- Master of Pathology and Pathophysiology, Peking Union Medical College, Chinese Academy of Medical Sciences, Sep. 2023 - Present
- Bachelor of Rehabilitation Therapeutics, Xuzhou Medical University, Sep. 2019 - June. 2023

## News 🔥 {#news}
- 2025.03: 🎉 RWKV-UI is accepted...</li>

## Publications 📄 {#publications}
{% assign pubs = site.publications | sort: 'date' | reverse %}
{% for pub in pubs limit:5 %}
<div style="display:flex; align-items:center; margin-bottom:20px; box-shadow:0 2px 6px rgba(0,0,0,0.1); padding:10px; border-radius:8px;">

  {% if pub.image %}
    <{div style="flex:0 0 200px; margin-right:20px;">
      <img src="{{ pub.image | relative_url }}" alt="{{ pub.title }}" style="max-width:100%; border-radius:6px;">
    </div>
  {% endif %}
  
  <div style="flex:1;">
    <p><strong>{{ pub.title }}</strong></p> 
    <p>{{ pub.citation }} </p> 
    <p>
      {% if pub.paperurl %}[PDF]({{ pub.paperurl }}){% endif %}
      {% if pub.bibtexurl %}[BibTeX]({{ pub.bibtexurl }}){% endif %}
    </p>
  </div>
</div>
{% endfor %}


