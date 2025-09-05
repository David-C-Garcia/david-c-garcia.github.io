---
layout: archive
title: "Selected Publications"
permalink: /publications/
author_profile: true
header:
  og_image: "images/profile.png"
---

<style>
/* Modern styling for publications page - matching research page */
.publications-container {
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

.text-block {
  background-color: #f9f9f9;
  border-left: 4px solid #4285f4;
  padding: 1.5em;
  margin: 2em 0;
  border-radius: 0 8px 8px 0;
}

.publication-item {
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 3px 10px rgba(0,0,0,0.08);
  margin-bottom: 1.5em;
  padding: 1.5em;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.publication-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 15px rgba(0,0,0,0.1);
}

/* Style the default archive single template output */
.archive__item-title {
  margin-top: 0 !important;
  font-size: 1.1em !important;
  font-weight: 600 !important;
}

.page__content .archive__item-title {
  margin-top: 0 !important;
  padding-bottom: 0 !important;
}

.archive__item-excerpt {
  font-size: 1em !important;
  line-height: 1.6 !important;
}

/* Make sure the publication list looks good */
.archive > ul {
  list-style-type: none !important;
  padding: 0 !important;
}

.archive > ul > li {
  margin-bottom: 1.5em !important;
}

/* Add styling to all publication entries */
.list__item {
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 3px 10px rgba(0,0,0,0.08);
  margin-bottom: 1.5em;
  padding: 1.5em;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.list__item:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 15px rgba(0,0,0,0.1);
}

/* Responsive styling */
@media screen and (max-width: 768px) {
  .publications-container {
    padding: 0 1em;
  }
}
</style>

<div class="publications-container">
  <p style="text-align: justify; font-size: 1.05em; line-height: 1.6;">
    Below is a list of selected publications and preprints. These works represent my research contributions in cell-free synthetic biology, biomanufacturing, and computational approaches to biological engineering.
  </p>

  <div class="text-block">
    <p style="text-align: justify; font-size: 1.1em; line-height: 1.6; margin: 0;">
      <b>For a full list of my publications, please see <a href="https://scholar.google.com/citations?user=HTLatcMAAAAJ&hl=en" target="_blank" rel="noopener">my Google Scholar page</a>.</b>
    </p>
  </div>

  <h2 class="section-heading">Publications</h2>

  {% include base_path %}

  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
</div>

