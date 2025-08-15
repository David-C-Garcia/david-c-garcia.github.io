---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
header:
  og_image: "images/profile.png"
---

<style>
/* Custom styling for research thumbnails - centered with even spacing */
.grid__wrapper {
  display: flex !important;
  flex-wrap: wrap !important;
  justify-content: center !important; /* Center the items */
  align-items: flex-start !important;
}
.grid__item {
  width: 28% !important; /* Slightly smaller to ensure all fit on one line */
  margin: 0 2% 20px 2% !important; /* Even margins on both sides */
}
@media screen and (max-width: 768px) {
  .grid__item {
    width: 45% !important;
    margin: 0 2% 20px 2% !important;
  }
}
@media screen and (max-width: 480px) {
  .grid__item {
    width: 90% !important;
    margin: 0 5% 20px 5% !important;
  }
}
</style>

<p style="text-align: justify;">
Engineerable biological systems have the potential to be some of our greatest tools against a host of problems, from biological and chemical threats to human health, to food insecurity, and the sustainable production of materials. Understanding the fundamental building blocks of complex biological systems and their interactions lies at the heart of creating biological tools that can function robustly, predictably, and with quantitative precision. However, the fundamental knowledge and high-throughput techniques to select ideal biocatalysts, reaction conditions, and production platforms are limited.
</p>

<p style="text-align: justify;">
The open nature of cell-free systems enables this work through a modular approach to biological transformations that allows for distinct biological components to be characterized rapidly and with precise control of the chemical environment. These methods reconceptualize how biological systems are engineered for applications in health, materials, and energy. Instead of making concessions between the cell's physiological and evolutionary objectives compared to engineerable objectives, we are able to rapidly test components and conditions, port them to cellular chassis, or use them directly in cell-free biomanufacturing platforms.
</p>

<p style="text-align: justify;">
<b>My lab will focus on developing new strategies that expand our traditional models of biomanufacturing sensors, materials, and molecules by taking a data-driven and multiplexed approach to elucidate the fundamental principles of scalable cell-free synthetic biology.</b>
</p>

<p align="center">
  <img src="/images/Current_work_melanin.png" width="900">
</p>

<p style="text-align: justify;">
My current project focuses on the use of protein language models to interrogate the substrate specificity and promiscuity of novel biocatalysts, using melanin as a model system for the large-scale production of biological polymers. This approach not only takes advantage of powerful pretrained protein language models but also makes effective use of high-throughput empirical verification to corroborate and fine-tune computational workflows.
</p>

<p style="text-align: justify;">
My future work will focus on three key projects to take a holistic approach to generating the tools and fundamental knowledge to develop cell-free systems as scalable biomanufacturing platforms and research tools: computationally driven design of biosensors, machine learning-enabled materials production, and fundamental explorations of cell-free metabolism towards small molecule production.
</p>

<nbsp>

{% include base_path %}

{% assign ordered_pages = site.research | sort:"order_number" %}

{% for post in ordered_pages %}
  {% include archive-single.html type="grid" %}
{% endfor %}
