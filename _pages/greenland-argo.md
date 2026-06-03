---
layout: archive
title: "Argo Floats in Greenland"
permalink: /research/greenland-argo/
author_profile: true
---

<!-- <div class="feature-hero">
  <p class="feature-kicker">Interactive Research Map</p>
  <h1>Argo Floats in on the Greenland Continental Shelf</h1>
  <p>
    Over the past several years, I've been working with Josh Willis at JPL to deploy autonomous profiling floats on the Greenland shelf.
  </p>
</div> -->

Over the past several years, I've been working with Josh Willis at JPL and Lorenz Meire at GINR to deploy autonomous profiling floats on the Greenland shelf. Sweet Zhang, software developer contributing to the CoOL group, has helped create tools to quality control data and ensure they are uploaded in the Argo DAC. Check out the recent data for these floats by clicking on their locations in the map below and following the links to the Argo DAC or the EuroArgo portal.

<link rel="stylesheet" href="https://js.arcgis.com/4.32/esri/themes/dark/main.css">
<script src="https://js.arcgis.com/4.32/"></script>

<div class="research-map-card">
  <div id="modelProjectMap"></div>
</div>

<script>
require([
  "esri/Map",
  "esri/views/MapView",
  "esri/layers/KMLLayer",
  "esri/widgets/Expand",
  "esri/widgets/BasemapGallery"
], function(Map, MapView, KMLLayer, Expand, BasemapGallery) {

  const kmlUrl = "https://mhwood.github.io/assets/kml/greenland-float-locations.kml?v={{ site.time | date: '%Y%m%d%H%M%S' }}";
  const map = new Map({
    basemap: "satellite"
  });

  const view = new MapView({
    container: "modelProjectMap",
    map: map,
    center: [-42, 70],
    zoom: 4,
    popup: {
      dockEnabled: true,
      dockOptions: {
        position: "bottom-right",
        breakpoint: false
      }
    }
  });

  const kmlLayer = new KMLLayer({
    url: kmlUrl,
    title: "Float Locations"
  });

  map.add(kmlLayer);

  kmlLayer.when(function() {
    view.goTo(kmlLayer.fullExtent).catch(function(error) {
      console.log(error);
    });
  });

  const basemapGallery = new BasemapGallery({
    view: view
  });

  const basemapExpand = new Expand({
    view: view,
    content: basemapGallery,
    expanded: false
  });

  view.ui.add(basemapExpand, "top-right");

});
</script>

<div class="feature-footer-card">
  <h2>Interested in this data?</h2>
  <p>
    More information about this effort can be found in the Arctic Report Card article Josh and I wrote in 2022 available <a href="https://doi.org/10.25923/b076-sj26">HERE</a>. You can also reach out to us to us directly if you have any questions. 
  </p>
  <a href="/research/">Back to research areas →</a>
</div>