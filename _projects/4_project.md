---
layout: page
title: Mapper
description: A tool that converts CSV datasets into knowledge graphs in TTL format, using a real-estate ontology to structure the information.
img: assets/img/mapper.PNG
importance: 2
category: work
giscus_comments: false
---

This module enables the construction and expansion of the Real Estate Knowledge Graph (OVS). The mapper processes structured data to generate a comprehensive knowledge graph (in .ttl format) containing all real estate entities and their associated information, ready for querying and analysis.

Originally, the mapper required the combination of two CSV files to run correctly. The module has now been refactored to operate flexibly based on the data source being integrated into the graph. It supports two execution modes, selected via command-line arguments:

--input_source scraper: Processes raw structured data from the scraper to build the initial knowledge graph.

--input_source ave: Enhances the existing graph (previously generated in scraper mode) by incorporating newly structured real estate features extracted via the Attribute Value Extraction (AVE) module. AVE is used to structure the unstructured data produced by the scraper, enabling richer and more detailed entity descriptions.

This modular design allows for incremental graph construction and refinement, ensuring seamless integration of data from different extraction stages without the need to manually merge CSV files beforehand.
