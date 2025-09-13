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
- 2025.03: 🎉 

## Publications 📄 {#publications}
{% assign pubs = site.publications | sort: 'date' | reverse %}
{% for pub in pubs limit:5 %}
<div class="pub-row">

  {% if pub.image %}
    <img src="{{ pub.image | relative_url }}" alt="{{ pub.title }}">
  {% endif %}
  
  <div class="pub-details">
    <p class="papertitle">{{ pub.title }}</p> 
    <p class="citation">{{ pub.citation }}</p> 
    <div class="pub-links">
      {% if pub.paperurl %}
        <a href="{{ pub.paperurl }}" download target="_blank">Paper</a>
      {% endif %}
      {% if pub.bibtexurl %}
        <a href="{{ pub.bibtexurl }}" target="_blank">BibTeX</a>
      {% endif %}
    </div>
  </div>
</div>
{% endfor %}


