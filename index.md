---
layout: default
title: Home
permalink: /
---

<!-- 完全恢复主题默认 Hero，只替换了 background、标题和副标题 -->
<section
  class="hero is-fullheight is-bold"
  style="background-image: url('{{ site.heroimage | relative_url }}');
         background-size: cover;
         background-position: center;"
>
  <div class="hero-body">
    <div class="container has-text-centered">
      <h1 class="title is-spaced">{{ site.title }}</h1>
      <h2 class="subtitle">{{ site.description }}</h2>
      <hr>
      <a
        href="{{ '/#about' | relative_url }}"
        class="button is-outlined is-inverted is-large"
      >
        Read More
      </a>
    </div>
  </div>
</section> 

