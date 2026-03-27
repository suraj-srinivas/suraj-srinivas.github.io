---
layout: default
title: publications
permalink: /publications
order: 1
---

<style>
.thesis-block {
  background: #ffffff;
  border-left: 4px solid #4a5568;
  border-radius: 0 8px 8px 0;
  box-shadow: 0 1px 6px rgba(0,0,0,0.07);
  padding: 0.8rem 1.4rem;
  margin-bottom: 1.2rem;
}
.section-heading {
  font-size: 1em;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.07em;
  color: #4a5568;
  border-bottom: 2px solid #e2e8f0;
  padding-bottom: 4px;
  margin-top: 1.8rem;
  margin-bottom: 0.8rem;
}
</style>

<div class="thesis-block">
<p>
<strong>phd thesis</strong><br>
<a href="https://infoscience.epfl.ch/record/289640">Gradient-based Methods for Deep Model Interpretability</a><br>
<em>École Polytechnique Fédérale de Lausanne (EPFL)</em><br>
2021 · <mark style="font-size:90%; padding:0px; margin:0px; background-color:transparent;">EPFL thesis distinction award (top 8%, EE dept.)</mark>
</p>
<!--
<p>
<strong>master thesis</strong><br>
<a href="pdfs/ms_thesis.pdf">Learning Compact Architectures for Deep Neural Networks</a><br>
<em>Indian Institute of Science (IISc)</em><br>
2017
</p>
-->
</div>

For more information see my [google scholar](https://scholar.google.com/citations?user=J2JWgKgAAAAJ) page. <u>Representative papers</u> are <mark style="background-color:mintcream">highlighted</mark> below.

<p class="section-heading">preprints</p>

{% include publications_2col.html type='preprint' %}
{% include publications_2col.html type='hack-to-avoid-tldr-error' %} 

<p class="section-heading">long papers</p>

{% include publications_2col.html type='long' %}
{% include publications_2col.html type='hack-to-avoid-tldr-error' %}

<p class="section-heading">short conference / workshop papers</p>

{% include publications_2col.html type='short' %}