---
layout: page
title: Geocoder
description: Geocoding script that generates geographic coordinates from textual address data.
img: assets/img/caminero.PNG
importance: 2
category: work
giscus_comments: false
---

This project processes and geocodes addresses using multiple Python libraries. It consists of three core scripts designed for flexibility and accuracy in converting addresses into geographic coordinates:

procesar_direcciones.py: Allows the user to select a CSV file and choose the preferred API for geocoding the addresses.

georreferenciar_direcciones.py: Handles batch conversion of addresses to geographic coordinates using the Georef API from DatosGobAr, with the option to select the number of addresses to process.

geolocalizar_con_delta.py: Adjusts addresses by adding 20 to their street numbers before geocoding, improving match accuracy in cases where slight address variations are needed.

The module is ideal for batch geocoding tasks, data enrichment, and spatial analysis—offering a reliable and customizable solution for transforming address data into actionable geographic insights.

For more info see: <a href="https://github.com/cientopolis/OVS-caminero">Geocoder Repository</a>
