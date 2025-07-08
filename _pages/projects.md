---
layout: page
title: Proyectos
permalink: /projects/
description: Descripción de los módulos que integran el Observatorio de Valores del Suelo
nav: true
nav_order: 3
---

# Equipos de Trabajo

## Infraestructura
**Coordinación:** Diego Torres
**Integrantes:**  
Alfonso Armani, David Matías, Justo Alvarado, Lucía Molina, Juli Ñancufil, Carolina Alonso, Beatriz Freitas, Tomás Bernardi, Pedro Artola, Joaquín Fontana

**Actividades:**
- Instalar Geonode, Geoserver y la base Postgres en forma nativa en su sistema operativo (preferentemente Linux)
- Instalación de Postgres en OKD
- Instalación de Geoserver y Geonode en OKD

## LLMs para construir grafos
**Coordinación:** Juana Borrelli  
**Integrantes:** Jesmar, Francisco Suárez, Fede (¿?), Iván González, Cosmos (¿?), Felipe Mass, Mate T (¿?)

## LLMs para construir consultas
**Coordinación:** Mateo Ibañez  
**Integrantes:** Migue Miesion, Luca Giordano, Francisco Suárez, Dylan Vallejos, Marcos Gerez, Matías Brizzi, Damián Bicocchi

## Manipulación del grafo
**Coordinación:** Alvaro Pagano  
**Integrantes:** Joaquín Sueyro, Mariano Vidal

## Visualización
**Coordinación:** Martín Venturino

---

# Módulos del Observatorio
![Modulos](/assets/img/projects/modulos.PNG)
## Scraper

![Scraper](/assets/img/projects/scraper.PNG)

El scraper es un script que permite obtener avisos inmobiliarios publicados en la web.

**Entrada:** --  
**Salida:** archivo CSV

---

## AVE

![AVE](/assets/img/projects/ave.PNG)

El Attribute Value Extraction es un programa que extrae pares atributo-valor a partir de descripciones de avisos inmobiliarios usando NLP.  
Proyecto basado en la tesina de Tanevitch y el Proyecto IDI 2024.

**Entrada:** CSV con descripciones de inmuebles  
**Salida:** CSV con características detectadas

---

## Caminero

![Caminero](/assets/img/projects/caminero.PNG)

El caminero genera coordenadas a partir de una dirección en texto (geocodificación).

**Entrada:** CSV con direcciones  
**Salida:** CSV con coordenadas detectadas

---

## Deduplicador

![Deduplicador](/assets/img/projects/deduplicador.PNG)

Permite hallar inmuebles duplicados. Hay dos versiones:

- **Sobre CSV:** utiliza un enfoque bayesiano que compara ciertos campos del archivo.
- **Sobre TTL:** enfoque inductivo/deductivo mediante *embeddings*.  
  Versión remasterizada en Python para ejecutar en Eva. Ver documento: _Graph Embeddings_

**Entrada:** CSV o TTL  
**Salida:** CSV con duplicados o TTL con URIs unificadas

---

## Mapper

![Mapper](/assets/img/projects/mapper.PNG)

Convierte un archivo CSV en un grafo de conocimiento en formato TTL usando una ontología inmobiliaria.

**Entrada:** CSV estructurado  
**Salida:** archivo TTL

---

## MillenniumDB
![MillenniumDB](/assets/img/projects/millenniumdb.PNG)
MillenniumDB es un gestor de grafos de conocimiento optimizado para manejar grafos masivos.

📎 [Repositorio en GitHub](https://github.com/MillenniumDB/MillenniumDB)

---

## GeoNode

![GeoNode](/assets/img/projects/geonode.PNG)

GeoNode es un software GIS.  
En 2024, se desplegó una instancia en el servidor del LIFIA con soporte para archivos `.csv`.

---

## QA (Question Answering)
![QA](/assets/img/projects/qa.PNG)

Técnica que permite realizar consultas en lenguaje natural sobre el grafo.  
Apunta a abstraerse del lenguaje SPARQL utilizando modelos de lenguaje (LLMs).

---

