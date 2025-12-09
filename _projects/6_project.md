---
layout: page
title: Deduplicator
description: A module designed to detect and merge duplicate real-estate listings to ensure clean and consistent data.
img: assets/img/deduplicador.PNG
importance: 6
category: work
---

This module addresses the challenge of identifying and removing duplicate real estate listings within the project's datasets. It leverages a knowledge graph ontology to represent property information obtained from scraped web data, and applies Knowledge Graph Embeddings (KGE) to detect duplicates in a scalable and semantically-aware way.

Using a trained KGE model, the system predicts a sameAs relationship between two property nodes, effectively determining whether they refer to the same real-world listing. This allows for automated deduplication, ensuring data consistency and improving the quality of the real estate knowledge graph.

The module removes redundant property entries, cleans the dataset, and maintains a single, accurate representation for each unique property—enhancing reliability for downstream analysis, reporting, and graph-based querying.