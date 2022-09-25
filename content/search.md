---
layout: page
title: Search
permalink: /search
---

<aside id="search-container">
  <input type="text" id="search-input" placeholder="Search blog posts..">
  <ul id="results-container"></ul>
</aside>
<script src="https://unpkg.com/simple-jekyll-search@latest/dest/simple-jekyll-search.min.js"></script>
<script>
var sjs = SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: '{{- "/search.json" | relative_url -}}'
})
</script>