---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
header:
  og_image: "images/profile.png"
---

<style>
/* Modern styling for research page */
.research-container {
  max-width: 1000px;
  margin: 0 auto;
}

.section-heading {
  font-size: 1.6em;
  color: #2a2a2a;
  margin: 1.8em 0 1em 0;
  padding-bottom: 0.4em;
  border-bottom: 2px solid #f2f2f2;
}

.highlight-text {
  background: linear-gradient(to bottom, transparent 50%, rgba(66, 133, 244, 0.15) 50%);
  padding: 0 4px;
}

.featured-image {
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  margin: 2em auto;
  transition: transform 0.3s ease;
  max-width: 100%;
  display: block;
}

.featured-image:hover {
  transform: translateY(-5px);
}

/* Custom styling for research thumbnails */
.grid__wrapper {
  display: flex !important;
  flex-wrap: wrap !important;
  justify-content: center !important;
  align-items: stretch !important;
  margin-top: 2em !important;
}

.grid__item {
  width: 28% !important;
  margin: 0 2% 30px 2% !important;
  border-radius: 8px !important;
  overflow: hidden !important;
  box-shadow: 0 3px 10px rgba(0,0,0,0.08) !important;
  transition: transform 0.3s ease, box-shadow 0.3s ease !important;
  background-color: #fff !important;
}

.grid__item:hover {
  transform: translateY(-5px) !important;
  box-shadow: 0 8px 15px rgba(0,0,0,0.1) !important;
}

.archive__item-teaser {
  position: relative;
  overflow: hidden;
}

.archive__item-teaser img {
  transition: transform 0.5s ease;
}

.grid__item:hover .archive__item-teaser img {
  transform: scale(1.05);
}

.archive__item-body {
  padding: 1em 1.2em !important;
}

.archive__item-title {
  margin-top: 0.5em !important;
  font-size: 1.1em !important;
  font-weight: 600 !important;
  line-height: 1.4 !important;
}

.text-block {
  background-color: #f9f9f9;
  border-left: 4px solid #4285f4;
  padding: 1.5em;
  margin: 2em 0;
  border-radius: 0 8px 8px 0;
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

<div class="research-container">
  <p style="text-align: justify; font-size: 1.05em; line-height: 1.6;">
  Engineerable biological systems have the potential to be some of our greatest tools against a host of problems, from biological and chemical threats to human health, to food insecurity, and the sustainable production of materials. Understanding the fundamental building blocks of complex biological systems and their interactions lies at the heart of creating biological tools that can function robustly, predictably, and with quantitative precision. However, the fundamental knowledge and high-throughput techniques to select ideal biocatalysts, reaction conditions, and production platforms are limited.
  </p>

  <p style="text-align: justify; font-size: 1.05em; line-height: 1.6;">
  The open nature of cell-free systems enables this work through a modular approach to biological transformations that allows for distinct biological components to be characterized rapidly and with precise control of the chemical environment. These methods reconceptualize how biological systems are engineered for applications in health, materials, and energy. Instead of making concessions between the cell's physiological and evolutionary objectives compared to engineerable objectives, we are able to rapidly test components and conditions, port them to cellular chassis, or use them directly in cell-free biomanufacturing platforms.
  </p>

  <div class="text-block">
    <p style="text-align: justify; font-size: 1.1em; line-height: 1.6; margin: 0;">
    <b>My lab will focus on developing new strategies that expand our traditional models of biomanufacturing sensors, materials, and molecules by taking a data-driven and multiplexed approach to elucidate the fundamental principles of scalable cell-free synthetic biology.</b>
    </p>
  </div>

  <img src="/images/Current_work_melanin.png" class="featured-image" alt="Current work on melanin production">

  <h2 class="section-heading">Current Research</h2>
  <p style="text-align: justify; font-size: 1.05em; line-height: 1.6;">
  My current project focuses on the use of <span class="highlight-text">protein language models</span> to interrogate the substrate specificity and promiscuity of novel biocatalysts, using melanin as a model system for the large-scale production of biological polymers. This approach not only takes advantage of powerful pretrained protein language models but also makes effective use of high-throughput empirical verification to corroborate and fine-tune computational workflows.
  </p>

  <h2 class="section-heading">Future Directions</h2>
  <p style="text-align: justify; font-size: 1.05em; line-height: 1.6;">
  My future work will focus on three key projects to take a holistic approach to generating the tools and fundamental knowledge to develop cell-free systems as scalable biomanufacturing platforms and research tools: 
  </p>
  <ul style="line-height: 1.6; font-size: 1.05em; margin-left: 1.5em;">
    <li>Computationally driven design of biosensors</li>
    <li>Machine learning-enabled materials production</li>
    <li>Fundamental explorations of cell-free metabolism towards small molecule production</li>
  </ul>

  <h2 class="section-heading">Research Projects</h2>

  {% include base_path %}
  {% assign ordered_pages = site.research | sort:"order_number" %}
  {% for post in ordered_pages %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>
