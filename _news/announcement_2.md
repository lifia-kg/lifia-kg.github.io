---
layout: post
title: Expo Ciencia y Tecnología 2025 - Informatica UNLP
date: 2025-10-22 09:11:00-0400
inline: false
related_posts: false
---
Motivation
---
The LIFIA Knowledge-Graph Team participated in ExpoCiencia 2025, showcasing recent advances in the development of knowledge-driven technologies for territorial analysis. Our presentation focused on the work carried out within the Land Value Observatory of the Province of Buenos Aires (OVS), a joint research initiative between LINTA, LIFIA, and the Provincial Agency for Social and Urban Integration (OPISU).


The OVS aims to monitor the evolution and conditions of parcels and real-estate assets across the Province of Buenos Aires. To achieve this, it requires an updated, georeferenced, and semantically enriched data infrastructure.

LIFIA contributed by developing the first version of a real-estate knowledge graph (KG) that powers the OVS platform. One of the ongoing challenges is enabling natural-language interaction with the graph so that non-expert users can benefit from the reasoning and inference capabilities of knowledge graphs.


---
# Work Presented at ExpoCiencia 2025
### 1. Integration Application with RDFGraphGPT

We developed an integration with RDFGraphGPT, an application that automatically translates natural language text into RDF knowledge graph structures using ChatGPT-5.
This tool brings together several components of our work:

Visualizing the OVS knowledge graph

Adding new instances directly from natural language

Asking natural-language questions to the KG

Automatically generating the corresponding SPARQL queries

Displaying results both as text (via a RAG pipeline) and graph-based visualizations

This provides a seamless workflow for querying, extending, and inspecting the knowledge graph.

### 2. Knowledge Graph Construction

We refactored the module responsible for constructing the real-estate knowledge graph from tabular property-listing data.
The new version supports two execution modes —Scraper and AVE— eliminating the need to manually merge intermediate files from different extraction processes. This optimization streamlines data integration and reduces the risk of inconsistencies.

### 3. Automatic SPARQL Query Generation

We trained ChatGPT-5 to transform natural-language questions into SPARQL queries over the real-estate KG. Using an example-based learning approach, the model learned the structure and patterns of the queries, achieving more accurate and consistent results.

During experimentation, we observed that small wording adjustments—such as using clearer synonyms—significantly improved the model’s interpretation.
We also defined a fixed context and a set of simple rules to guide query generation, reducing ambiguity and increasing reliability and stability.

### 4. RAG Pipeline Implementation

The RAG system integrates two AI models working in sequence:

GPT-5 converts the user’s question into a SPARQL query.

The query is executed on MillenniumDB, retrieving the relevant RDF triples.

Llama-3 interprets those triples and generates a coherent, context-aware answer in natural language.

This approach allows users to ask complex questions and receive easily understandable responses without needing SPARQL expertise.

### 5. Web Interface Enhancements for GeoNode

We improved the design and usability of GeoNode, the geospatial data management platform used in the OVS ecosystem. Enhancements include:
<ul>
    <li>A cleaner, streamlined interface</li>
    <li>Integration of custom images and logos</li>
    <li>Removal of unnecessary elements</li>
    <li>Better navigation and overall user experience</li>
</ul>

These improvements support a more intuitive and visually consistent interaction with OVS datasets.