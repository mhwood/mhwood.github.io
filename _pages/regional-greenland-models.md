---
layout: archive
title: "Regional Greenland Models"
permalink: /research/regional-greenland-models/
author_profile: true
---

<div class="feature-hero">
  <p class="feature-kicker">Research Feature</p>
  <h1>Glacier-Ocean Interactions in Four Greenland Regions</h1>
  <p>
    Explore the following regional models that encompass the entirety of the Greenland coastline. These regional models were constructed on portions of the "Lat-Lon-Cap" grids.
  </p>
</div>

<div class="scrolly-wrapper">

  <div class="scrolly-text">

    <section class="scrolly-step is-active"
             data-image="/images/research/regional-models/ce_model_example_field.png"
             data-caption="Potential Temperature in the CE Greenland Configuration">
      <div class="step-card">
        <span class="step-number">CE</span>
        <h2>Central East Greenland</h2>
        <p>
          This model encompasses the East Greenland current and includes glaciers from Kangerlussuaq through 79N. The grid is formed on a portion of ECCO's LLC1080 grid.
        </p>
        
        <h3><a href="https://doi.org/10.1029/2023GL107983">Article →</a></h3>
        <h3><a href="https://github.com/mhwood/downscale_greenland/tree/main/L1/L1_CE_Greenland">Model Code →</a></h3>
      </div>
    </section>

    <section class="scrolly-step"
             data-image="/images/research/circulation.jpg"
             data-caption="Potential Temperature in the W Greenland Configuration">
      <div class="step-card">
        <span class="step-number">W</span>
        <h2>West Greenland</h2>
        <p>
          This model encompasses West Greenland includes glaciers from the southern-most fjords through Qimusersiarsuaq (Melville Bay).
        </p>
      </div>
    </section>

    <section class="scrolly-step"
             data-image="/images/research/regional-models/se_model_example_field.png"
             data-caption="Potential Temperature in the SE Greenland Configuration">
      <div class="step-card">
        <span class="step-number">SE</span>
        <h2>Southeast Greenland</h2>
        <p>
          This model encompasses the East Greenland and Irmginer currents and includes glaciers from the southern-most fjords through Kangerlussuaq.
        </p>
      </div>
    </section>

    <section class="scrolly-step"
             data-image="/images/research/regional-models/n_model_example_field.png"
             data-caption="Potential Temperature in the N Greenland Configuration">
      <div class="step-card">
        <span class="step-number">N</span>
        <h2>North Greenland</h2>
        <p>
          This model encompasses the fjords around northern Greenland.
        </p>
      </div>
    </section>

  </div>

  <div class="scrolly-visual">
    <div class="sticky-figure">
      <img id="scrolly-image"
           src="/images/research/model-domain.jpg"
           alt="Research feature image">
      <div id="scrolly-caption" class="figure-caption">
        Model domain and fjord-scale bathymetry
      </div>
    </div>
  </div>

</div>

<div class="feature-footer-card">
  <h2>Interested in these models?</h2>
  <p>
    Please reach out! I am happy to share all input binaries and other files necessary for you to run these models on your own.
  </p>
  <a href="/research/">Back to research areas →</a>
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const steps = document.querySelectorAll(".scrolly-step");
  const image = document.getElementById("scrolly-image");
  const caption = document.getElementById("scrolly-caption");

  if (!steps.length || !image || !caption) return;

  const observer = new IntersectionObserver(
    entries => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          const step = entry.target;
          const nextImage = step.dataset.image;
          const nextCaption = step.dataset.caption;

          steps.forEach(s => s.classList.remove("is-active"));
          step.classList.add("is-active");

          image.classList.add("is-fading");

          setTimeout(() => {
            image.src = nextImage;
            caption.textContent = nextCaption;
            image.classList.remove("is-fading");
          }, 180);
        }
      });
    },
    {
      root: null,
      threshold: 0.55
    }
  );

  steps.forEach(step => observer.observe(step));
});
</script>