---
title: Officers
layout: default
nav_order: 2
description: A listing of all the club officers
---

# Officers

A list of current and past people helping run the go club.

## Current

{% for officer in site.officers %}
<div class="officer">
  <img class="officer-image" src="{{ site.baseurl }}assets/images/{{ officer.photo }}" alt="">

  <div>
    <h3 class="officer-name">
      {{ officer.display_name }}
      {% if officer.role %} 
	- {{ officer.role }}
      {% endif %}

      {% if officer.pronouns %}
        <span class="officer-pronouns">{{ officer.pronouns }}</span>
      {% endif %}
    </h3>

    {{ officer.content }}
  </div>
</div>
{% endfor %}

## Archives

### Fall 2014
- Curtis Tang
- Yuxuan Luo
- Peter Kim
- Qingen Zhang
- Jun Zhang

### Fall 2013
- Yilin Wei
- Chengwei Wang
- Chenyu Song
- Zhiye Wang
- Yuxuan Luo
- Yunpeng Yu
- Huirong Zhu
- Zhuoran Li
