---
layout: post
title: Home
permalink: /
---

<nav>
  <ul>
{%- for post in site.posts -%}
    <li>
      <h2><a href="{{- post.url | relative_url -}}">{{- post.title -}}</a></h2>
    </li>
{%- endfor -%}
  </ul>
</nav>
