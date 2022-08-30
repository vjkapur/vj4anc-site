---
title: "What is a school zone?"
permalink: /issues/schoolzones/
excerpt: "just asking questions"
author_profile: false
header:
  overlay_image: /assets/images/screaming.jpg
  overlay_filter: rgba(127, 127, 127, 0.5)
  caption: "[Screaming](/assets/images/screaming.jpg)"
categories: investigating
# toc: true
toc_label: "Page Contents"
toc_icon: "bullseye"
toc_sticky: true
last_modified_at: 2022-08-30T00:21:06
---
<div id="map" class="map-container"></div>

<script>
var map = L.map('map',  {
      zoomSnap: 0.25
  }).setView([38.924951694539075, -76.9770712988049], 17);
  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      maxZoom: 19,
      attribution: '© OpenStreetMap'
  }).addTo(map);

  //var circle = L.circle([38.925566108416504, -76.9789891588733], {radius: 100}).addTo(map);

  var building = L.polygon([[38.92465337392036, -76.97730491637637], [38.92494212905769, -76.97730491637637], [38.92494212905769, -76.97732487144394], [38.925233987894686, -76.97730491637637], [38.92524019764415, -76.97704949151147], [38.92515015622399, -76.97705348252498], [38.92514705134539, -76.97676213853842], [38.92529298049247, -76.97673819245735], [38.92532092433745, -76.97649474063297], [38.925035275625476, -76.97651070468703], [38.92502204039862, -76.97648673084626], [38.92466249425416, -76.976502805939]], {color: 'darkred'}).addTo(map)

  var groundsLatLong = [[38.92553127340432, -76.9762473715858], [38.92553268276262, -76.9774063214896], [38.92468744001965, -76.97821685328435], [38.92453686734274, -76.97821739728843],[38.92453501755463, -76.97619542422468], [38.924647718571634, -76.97624909891559], [38.92553127340432, -76.9762473715858]]

  var grounds = L.polygon(groundsLatLong, {color: 'red'}).addTo(map);

  for (var i = 0; i < groundsLatLong.length; i++) {
    L.circle(groundsLatLong[i], {radius: (.9144*100), stroke: false}).addTo(map);
    //L.circle(groundsLatLong[i], {radius: (.9144*150), stroke: false}).addTo(map);
  }



</script>