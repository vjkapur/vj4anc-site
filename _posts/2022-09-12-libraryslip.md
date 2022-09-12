---
title: "9/22 TSIs"
permalink: /issues/tsis-202209/
excerpt: "#AllForAllie"
author_profile: false
header:
  overlay_image: /assets/images/woodridge-library-roof.jpg
  overlay_filter: rgba(127, 127, 127, 0.5)
  caption: "[placeholder](/assets/images/woodridge-library-roof.jpg)"
categories: proactive requesting
# toc: true
toc_label: "Page Contents"
toc_icon: "bullseye"
toc_sticky: true
last_modified_at: 2022-09-04T02:52:42
---
<div id="tsi-map" class="map-container"></div>

*[TSI]: Traffic Safety Investigation

<script>
var map = L.map('tsi-map',  {
      zoomSnap: 0.25
  }).setView([38.927709339916234, -76.97851570614057], 19);
  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      maxZoom: 19,
      attribution: '© OpenStreetMap'
  }).addTo(map);

  woodridgeSlipLonLat = [[-76.97867818962725, 38.92775700991655],[-76.97861227435399, 38.927726601950894],[-76.97831741986357, 38.92772451921303],[-76.97829081211528, 38.92769333154149],[-76.97863749542395, 38.92769979337186],[-76.97871968014083, 38.927739621731234],[-76.97867818962725, 38.92775700991655]]

  woodridgeSlipLatLon = []
  for (var i = 0; i < woodridgeSlipLonLat.length; i++) {
    woodridgeSlipLatLon.push([woodridgeSlipLonLat[i][1], woodridgeSlipLonLat[i][0]]);
  }

  var polygon = L.polygon(woodridgeSlipLatLon, {color: 'red'}).addTo(map);
</script>