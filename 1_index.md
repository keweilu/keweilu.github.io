---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: page
title: Home
permalink: /
order: 1
---

<header class="website-header">
    {% if site.portrait %}
      <a class="portrait" href="{{site.url}}{{site.baseurl}}" style="background-image: url('{{ site.portrait | prepend: site.baseurl }}')"></a>
      <!-- <img src="{{ site.portrait | relative_url }}" class="mx-auto d-block rounded-circle" alt="portrait" width="150" height="150" style="margin-top: 60px; margin-bottom: 20px;"> -->
    {% endif %}
    <!-- <h1 class="blog-title">{{ site.configuration.title }}</h1> -->
    &nbsp;&nbsp;&nbsp;&nbsp;
    <div class="custom-links">
      {% for social in site.social %}
        {% if social.icon == "scholar" %}
            <a href="{{ social.url }}" {% if social.desc %} title="{{ social.desc }}"{% endif %} target="_blank" role="button">
              <i class="ai ai-google-scholar-square ai-3x ai-fw"></i>
            </a>
        {% elsif social.icon == "envelope-square" %}
          <a href="mailto:{{ social.url }}" title="{{ social.desc }}">
            <i class="fas fa-{{ social.icon }} fa-3x fa-fw"></i>
          </a>
        {% else %}
            <a href="{{ social.url }}" {% if social.desc %} title="{{ social.desc }}"{% endif %} target="_blank" role="button">
              <i class="fab fa-{{ social.icon }} fa-3x fa-fw"></i>
            </a>
        {% endif %}
      {% endfor %}
    </div>
</header>


Kewei Lu currently works at [GoDaddy](https://www.godaddy.com/) in San Francisco Bay Area. He received his Ph.D in Computer Science and Engineering [Computer Science and Engineering](https://cse.osu.edu/) from The Ohio State University. His advisor is [Prof. Han-Wei Shen](http://web.cse.ohio-state.edu/~hwshen/hwshen/Welcome.html). His research interests are large scale data visualization, high performance computing and interactive visualization.  

Kewei Lu received his bachelor degree in Computer Science and Technology at [Wuhan University of Technology](http://english.whut.edu.cn/) in 2009 and master degree in Computer Science and Engineering at [The Ohio State University](https://www.osu.edu/) in 2011.
