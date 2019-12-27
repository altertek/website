---
layout: splash
namespace: index
title: ""
classes: wide
header:
  overlay_image: "/assets/images/header.png"
  overlay_color: "#fff"
---

{% translate_file index.md %}

<div class="feature__wrapper">

{%- for item in site.translations[site.lang]["index"] -%}
    <div class="feature__item">
      <div class="archive__item">
          <div class="archive__item-teaser">
            <img src="{{ item.image_path }}" alt="{{ item.title }}" />
          </div>
        <div class="archive__item-body">
            <h2 class="archive__item-title">{{ item.title }}</h2>
            <div class="archive__item-excerpt">
              <p>{{ item.excerpt }}</p>
            </div>
        </div>
      </div>
    </div>
{%- endfor -%}

</div>
