---
title: "Rhode Island Avenue bus priority lanes"
permalink: /issues/riabuslanes/
excerpt: "I didn't realize there'd be so many"
author_profile: false
header:
  overlay_filter: rgba(127, 127, 127, 0.5)
  overlay_image: /assets/images/RIA-at-night.jpg
  caption: "[Rhode Island Ave. at night](/assets/images/RIA-at-night.jpg)"
categories: initiatives
---

<div id="ria-map" class="map-container"></div>

<script>
var map = L.map('ria-map',  {
      zoomSnap: 0.25
  }).setView([38.92149505828077, -76.99584577421773], 13);
  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      maxZoom: 19,
      attribution: '© OpenStreetMap'
  }).addTo(map);

  var eastern_to_logan = L.polygon([[38.93528521651921, -76.96358022990226], [38.924708977903684, -76.98560186514584], [38.921781259389896, -76.9949781650645], [38.92151509718208, -76.99591579512335], [38.92052930253024, -76.99876669732937], [38.91001988020146, -77.02889756491636], [38.909802971421506, -77.02883421153402], [38.920292709802816, -76.9986526613931], [38.92110106512349, -76.99618187948121], [38.924452684050564, -76.98553851124541], [38.924501971408276, -76.98543714617414], [38.93507824097857, -76.96335215790336]], {color: 'red'}).addTo(map);

  var logan_circle = L.circle([38.90962533031907, -77.02963006996238], {radius: 70, color: 'red'}).addTo(map);

  var logan_to_15th = L.polygon([[38.90952090321756, -77.03035379071768], [38.908025397328274, -77.03462934116963], [38.90788045675677, -77.03443461312924], [38.90932984915458, -77.03027759278885]], {color: 'red'}).addTo(map);
</script>

## SMDs that touch or contain RIA
Consider Eastern Ave. to 15th St NW for now. The Bus Priority Corridor ends at 14th (but no SMD does)

|SMD|election status|segment (east-west)|side|
|---|---|---|---|
|5B07|contested|Eastern to South Dakota|both|
|5B06|uncontested(+)|South Dakota to 16th NE|north|
|5C07|uncontested(+)|South Dakota to Evarts NE|south|
|5B03|uncontested(+?)|16th NE to 13th NE|north|
|5C06|uncontested(-?)|Evarts NE to Brentwood|south|
|5B04|contested(+?)}|13th NE to Met Branch|north|
|5C05|uncontested(+?)|Brentwood to Met Branch|south|
|5F03|uncontested(-)|Met Branch to 4th NE|north|
|5F06|uncontested(+?)|Met Branch to 4th NE|south|
|5F04|contested|4th NE to Lincoln|both/north|
|5F05|contested|Summit to Lincoln|south|
|5F07|contested|Lincoln to North Cap|south|
|5E04|contested|Lincoln to 2nd NW|north/both/north|
|5E03|uncontested(?)|T NW to Florida|south|
|5E02|contested|Florida to New Jersey Ave|south|
|1B01|uncontested|2nd NW to New Jersey|north|
|2G01|contested|New Jersey to 11th NW|north|
|2G03|contested|New Jersey to 7th NW|south|
|2G02|contested|7th NW to 11th NW|south|
|2F07|uncontested|11th to Logan Circle|both|
|2F03|no candidate|Logan Circle to 15th|north|
|2F04|uncontested(?)|Logan Circle to 15th|north|