---
layout: default
title: CV
lang: fr
---

<nav>
  <a href="/fr/">À propos</a> 
  <a href="/fr/research">Recherche</a>
  <a href="/fr/code">Code</a>
  <a href="/fr/cv">CV</a>
</nav>

<style>
.cv-container {
  display: flex;
  justify-content: center;
  margin: 2rem auto;
  max-width: 900px;
}
.cv-frame {
  width: 100%;
  height: 85vh;      /* 85% de la hauteur de la fenêtre */
  border: 1px solid #ccc;
  border-radius: 4px;
}
</style>

<div class="cv-container">
<iframe 
    src="{{ '/assets/pdf/CV_website_FR.pdf' | relative_url }}"
    class="cv-frame">
</iframe>
</div>
