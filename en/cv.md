---
layout: default
title: CV
lang: en
---

<nav>
  <a href="/en/">Home</a>
  <a href="/en/research">Research</a>
  <a href="/en/code">Code</a>
  <a href="/en/cv">CV</a>
</nav>

Le problème vient du fait que ton <iframe> n'a pas de hauteur définie : par défaut, un iframe fait environ 150px de haut, d'où l'aspect minuscule. Il faut lui donner une taille explicite en CSS.

Voici ton code ajusté avec un bloc <style> intégré :

html
---
layout: default
title: CV
lang: en
---
<nav>
  <a href="/en/">Home</a>
  <a href="/en/research">Research</a>
  <a href="/en/code">Code</a>
  <a href="/en/cv">CV</a>
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
    src="{{ '/assets/pdf/CV_website_EN.pdf' | relative_url }}"
    class="cv-frame">
</iframe>
</div>
