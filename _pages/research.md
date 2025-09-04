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

.research-intro {
  position: relative;
  margin-bottom: 3em;
}

.highlight-text {
  font-weight: 700;
  color: #0056b3;
}

/* Animated underline for section titles */
.section-title {
  position: relative;
  display: inline-block;
  font-size: 1.6em;
  margin: 1.5em 0 1em 0;
  padding-bottom: 0.3em;
}

.section-title::after {
  content: '';
  position: absolute;
  width: 0;
  height: 3px;
  bottom: 0;
  left: 0;
  background-color: #0056b3;
  visibility: hidden;
  transition: all 0.3s ease-in-out;
}

.section-title.visible::after {
  visibility: visible;
  width: 100%;
}

/* Featured research image */
.featured-image {
  border-radius: 8px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  margin: 2em 0;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  max-width: 100%;
}

.featured-image:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 20px rgba(0,0,0,0.15);
}

/* Research card grid */
.grid__wrapper {
  display: grid !important;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr)) !important;
  gap: 2em !important;
  margin-top: 3em !important;
}

.grid__item {
  width: 100% !important;
  margin: 0 !important;
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
  border-radius: 8px 8px 0 0;
}

.archive__item-teaser img {
  transition: transform 0.5s ease;
}

.grid__item:hover .archive__item-teaser img {
  transform: scale(1.05);
}

.archive__item-title {
  margin-top: 0.5em !important;
  font-size: 1.2em !important;
  font-weight: bold !important;
}

/* Fade-in animation for elements */
.fade-in {
  opacity: 0;
  transform: translateY(20px);
  transition: opacity 0.6s ease-out, transform 0.6s ease-out;
}

.fade-in.visible {
  opacity: 1;
  transform: translateY(0);
}

/* Responsive adjustments */
@media screen and (max-width: 768px) {
  .grid__wrapper {
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr)) !important;
  }
}

@media screen and (max-width: 480px) {
  .grid__wrapper {
    grid-template-columns: 1fr !important;
  }
}
</style>

<div class="research-container">
  <section class="research-intro fade-in">
    <p style="text-align: justify;">
      Engineerable biological systems have the potential to be some of our greatest tools against a host of problems, from biological and chemical threats to human health, to food insecurity, and the sustainable production of materials. Understanding the fundamental building blocks of complex biological systems and their interactions lies at the heart of creating biological tools that can function robustly, predictably, and with quantitative precision. However, the fundamental knowledge and high-throughput techniques to select ideal biocatalysts, reaction conditions, and production platforms are limited.
    </p>

    <p style="text-align: justify;">
      The open nature of cell-free systems enables this work through a modular approach to biological transformations that allows for distinct biological components to be characterized rapidly and with precise control of the chemical environment. These methods reconceptualize how biological systems are engineered for applications in health, materials, and energy. Instead of making concessions between the cell's physiological and evolutionary objectives compared to engineerable objectives, we are able to rapidly test components and conditions, port them to cellular chassis, or use them directly in cell-free biomanufacturing platforms.
    </p>

    <p style="text-align: justify; font-size: 1.1em;" class="highlight-text">
      My lab will focus on developing new strategies that expand our traditional models of biomanufacturing sensors, materials, and molecules by taking a data-driven and multiplexed approach to elucidate the fundamental principles of scalable cell-free synthetic biology.
    </p>
  </section>

  <div class="featured-image-container fade-in">
    <img src="/images/Current_work_melanin.png" class="featured-image" alt="Current work on melanin production">
  </div>

  <section class="current-work fade-in">
    <h2 class="section-title">Current Research</h2>
    <p style="text-align: justify;">
      My current project focuses on the use of protein language models to interrogate the substrate specificity and promiscuity of novel biocatalysts, using melanin as a model system for the large-scale production of biological polymers. This approach not only takes advantage of powerful pretrained protein language models but also makes effective use of high-throughput empirical verification to corroborate and fine-tune computational workflows.
    </p>
  </section>

  <section class="future-work fade-in">
    <h2 class="section-title">Future Directions</h2>
    <p style="text-align: justify;">
      My future work will focus on three key projects to take a holistic approach to generating the tools and fundamental knowledge to develop cell-free systems as scalable biomanufacturing platforms and research tools: computationally driven design of biosensors, machine learning-enabled materials production, and fundamental explorations of cell-free metabolism towards small molecule production.
    </p>
  </section>

  <section class="research-projects fade-in">
    <h2 class="section-title">Research Projects</h2>
    
    {% include base_path %}
    {% assign ordered_pages = site.research | sort:"order_number" %}
    {% for post in ordered_pages %}
      {% include archive-single.html type="grid" %}
    {% endfor %}
  </section>
</div>

<script>
  // Intersection Observer for animations
  document.addEventListener('DOMContentLoaded', function() {
    const fadeElements = document.querySelectorAll('.fade-in, .section-title');
    
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
          observer.unobserve(entry.target);
        }
      });
    }, {
      threshold: 0.2,
      rootMargin: '0px 0px -50px 0px'
    });
    
    fadeElements.forEach(element => {
      observer.observe(element);
    });
  });
</script>
