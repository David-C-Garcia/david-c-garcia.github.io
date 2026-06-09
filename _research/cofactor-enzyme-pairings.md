---
layout: single
title: "Predicting Cofactor–Enzyme Pairings with Protein Language Models"
collection: research
permalink: /research/cofactor-enzyme-pairings/
header:
  og_image: "images/Research_Images/cofactor_optimization_LLM.png"
---

<style>
.project-page {
  max-width: 980px;
  margin: 0 auto;
}

.project-hero {
  position: relative;
  overflow: hidden;
  margin: 0 0 2rem 0;
  padding: 1.9rem 2rem;
  border-radius: 18px;
  background: linear-gradient(135deg, #f0f7ff 0%, #ffffff 50%, #eef7f0 100%);
  box-shadow: 0 18px 40px rgba(15, 35, 56, 0.08);
}

.project-hero::before {
  content: "";
  position: absolute;
  top: -30px;
  right: -40px;
  width: 180px;
  height: 180px;
  border-radius: 50%;
  background: radial-gradient(circle, rgba(36, 102, 176, 0.2) 0%, rgba(36, 102, 176, 0) 72%);
}

.project-hero h1 {
  position: relative;
  z-index: 1;
  margin: 0;
  font-size: clamp(1.5rem, 2.5vw, 2.1rem);
  color: #18375a;
  line-height: 1.3;
}

.project-image-wrap {
  margin: 0 0 1.5rem 0;
  border-radius: 14px;
  overflow: hidden;
  border: 1px solid #dbe7f2;
  background: #ffffff;
  box-shadow: 0 14px 30px rgba(17, 40, 64, 0.08);
}

.project-image-wrap img {
  display: block;
  width: 100%;
  height: auto;
}

.project-body {
  margin: 0;
  padding: 0 0.2rem;
}

.project-body p {
  margin: 0;
  color: #2c3f55;
  font-size: 1.06rem;
  line-height: 1.85;
  text-align: justify;
}

@media (max-width: 768px) {
  .project-hero {
    padding: 1.4rem 1.2rem;
  }

  .project-body p {
    font-size: 1rem;
    line-height: 1.75;
  }
}
</style>

<div class="project-page">
  <section class="project-hero">
    <h1>Predicting Cofactor–Enzyme Pairings with Protein Language Models</h1>
  </section>

  <figure class="project-image-wrap">
    <img src="{{ '/images/Research_Images/cofactor_optimization_LLM.png' | relative_url }}" alt="Workflow for predicting cofactor-enzyme pairings with protein language models">
  </figure>

  <section class="project-body">
    <p>
      Biological catalysts often require specific conditions and cofactors in order to function optimally. Identifying the right enzyme–cofactor pairings has traditionally relied on titrations of individually purified enzymes, limiting throughput and leaving many biocatalysts uncharacterised. As part of understanding the cofactor needs of industrially relevant enzymes we are making use of cell-free synthetic biology, high throughput liquid handling, and protein-language models to measure the cofactor needs of polyphenol oxidases.
    </p>
  </section>
</div>
