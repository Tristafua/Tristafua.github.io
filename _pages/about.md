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
- 2023.09 - Present, Peking Union Medical College / Chinese Academy of Medical Sciences
  Master of Pathology and Pathophysiology
- 2019.09 - 2023.06, Xuzhou Medical University
  Bachelor of Rehabilitation Therapeutics

## News 🔥 {#news}
- 2025.03: 🎉 

## Publications 📄 {#publications}
{% assign pubs = site.publications | sort: 'date' | reverse %}
{% for pub in pubs limit:6 %}
<div class="pub-item">

  {% if pub.image %}
  <div class="pub-thumb">
    <img src="{{ pub.image | relative_url }}" alt="{{ pub.title }}">
  </div>
  {% endif %}

  <div class="pub-body">
    <h3 class="pub-title">
      {% if pub.paperurl %}
        <a href="{{ pub.paperurl }}" target="_blank">{{ pub.title }}</a>
      {% else %}
        {{ pub.title }}
      {% endif %}
    </h3>

    {% if pub.authors %}
      <p class="pub-authors">{{ pub.authors }}</p>
    {% else %}
      <p class="pub-authors">{{ pub.citation }}</p>
    {% endif %}

    <p class="pub-links">
      {% if pub.codeurl %}<a href="{{ pub.codeurl }}" target="_blank">Code</a>{% endif %}
      {% if pub.paperurl %}<a href="{{ pub.paperurl }}" download target="_blank">Paper</a>{% endif %}
      {% if pub.videourl %}<a href="{{ pub.videourl }}" target="_blank">Video</a>{% endif %}
      {% if pub.bibtexurl %}<a href="{{ pub.bibtexurl }}" target="_blank">BibTeX</a>{% endif %}
    </p>
  </div>

</div>
{% endfor %}
