---
layout: single
title: "Bus Route Access Heatmap in Dhaka"
permalink: /bus-access-heatmap/
author_profile: true
---

This project analyzes and visualizes the spatial intensity of bus service coverage across Dhaka using scraped route data, geocoded bus stops, clustering, and GIS heatmap generation. The objective was to identify well-served areas and detect underserved zones through both service intensity and population overlays.

---

### Key Steps

- **Web scraping**: Collected bus routes and stop sequences from a Dhaka-specific transit website.
- **Geocoding**: Converted unique stop names into coordinates using OpenStreetMap Nominatim API.
- **Fuzzy matching**: Mapped geocoded coordinates to the full stop list using fuzzy string matching.
- **Clustering**: Applied DBSCAN on lat/lon data to group stops within 500 meters and count unique services per cluster.
- **GIS visualization**: Used QGIS to generate a heatmap of service intensity, overlay with population data (WorldPop), and highlight underserved high-density areas.

---

### Tools Used

- Python (pandas, geopy, fuzzywuzzy, scikit-learn)
- QGIS 3.40.5
- OpenStreetMap basemap
- WorldPop 1 km-resolution raster

---

### Repository
 
[GitHub Repository – Bus Route Access Heatmap](https://github.com/muhtashimshahrier/dhaka-bus-access-heatmap)

---

