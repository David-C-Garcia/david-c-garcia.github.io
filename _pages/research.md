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

.research-hero {
  position: relative;
  margin: 0 0 2em 0;
  padding: 2em 2.2em;
  border-radius: 20px;
  background: linear-gradient(135deg, #f4f8ff 0%, #ffffff 55%, #eef6f0 100%);
  box-shadow: 0 18px 40px rgba(24, 44, 72, 0.08);
  overflow: hidden;
}

.research-hero::after {
  content: "";
  position: absolute;
  top: -40px;
  right: -20px;
  width: 180px;
  height: 180px;
  border-radius: 50%;
  background: radial-gradient(circle, rgba(66, 133, 244, 0.18) 0%, rgba(66, 133, 244, 0) 70%);
}

.research-hero__text {
  position: relative;
  z-index: 1;
  margin: 0;
  color: #20324d;
  font-size: 1.2em;
  line-height: 1.7;
}

.research-figure {
  margin: 1.5em 0 2em 0;
}

.research-figure img {
  display: block;
  width: 100%;
  height: auto;
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
  display: flex !important;
  width: 28% !important;
  margin: 0 2% 30px 2% !important;
  border-radius: 8px !important;
  overflow: hidden !important;
  box-shadow: 0 3px 10px rgba(0,0,0,0.08) !important;
  transition: transform 0.3s ease, box-shadow 0.3s ease !important;
  background-color: #fff !important;
}

.grid__item .archive__item {
  display: flex;
  flex-direction: column;
  width: 100%;
  height: 100%;
}

.grid__item:hover {
  transform: translateY(-5px) !important;
  box-shadow: 0 8px 15px rgba(0,0,0,0.1) !important;
}

.archive__item-teaser {
  position: relative;
  overflow: hidden;
  aspect-ratio: 16 / 10;
  background-color: #eef3f7;
}

.archive__item-teaser img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
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

@media screen and (max-width: 768px) {
  .research-hero {
    padding: 1.7em;
  }

  .research-hero__text {
    font-size: 1.1em;
  }

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
  <div class="research-hero">
    <p class="research-hero__text">
      <strong>Our lab develops new strategies that expand traditional models of biomanufacturing sensors, materials, and molecules through a data-driven, multiplexed approach that reveals the core principles of scalable cell-free synthetic biology.</strong>
    </p>
  </div>

  <p style="text-align: justify; font-size: 1.05em; line-height: 1.6;">
  Engineerable biological systems have the potential to be some of our greatest tools against a host of problems, from biological and chemical threats to human health, to food insecurity, and the sustainable production of materials. Understanding the fundamental building blocks of complex biological systems and their interactions lies at the heart of creating biological tools that can function robustly, predictably, and with quantitative precision. However, the fundamental knowledge and high-throughput techniques to select ideal biocatalysts, reaction conditions, and production platforms are limited.
  </p>

  <figure class="research-figure">
    <img src="{{ '/images/Research_Images/research_directions_image.png' | relative_url }}" alt="Illustration of the lab's research directions in cell-free synthetic biology">
  </figure>

  <p style="text-align: justify; font-size: 1.05em; line-height: 1.6;">
  The open nature of cell-free systems enables this work through a modular approach to biological transformations that allows for distinct biological components to be characterized rapidly and with precise control of the chemical environment. These methods reconceptualize how biological systems are engineered for applications in health, materials, and energy. Instead of making concessions between the cell's physiological and evolutionary objectives compared to engineerable objectives, we are able to rapidly test components and conditions, port them to cellular chassis, or use them directly in cell-free biomanufacturing platforms.
  </p>

