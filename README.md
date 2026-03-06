# URBAN-DATA-ANALYTICS: **INSTABILITY TERRITÓRIES**
This project aims to identify vulnerable areas in the urban fabric using Google Earth Engine to access, extract, cross-reference, and analyze satellite and GIS data in order to interpret the territory and identify areas at risk of flooding.

---
### **PROJECT INTENTION**

The project aims to identify environmentally vulnerable areas within the urban fabric of Teresópolis (Rio de Janeiro) through the integration of ecological, territorial, and geospatial data. Using spatial analysis and remote sensing tools, the research seeks to map riparian vegetation, analyze land occupation patterns, and identify areas exposed to flood risk. The workflow combines biological occurrence databases, satellite imagery, and GIS-based analytical methods to support territorial interpretation and inform potential design and planning strategies.

---

### **FILES DESCRIPTION**

> **00_BASE DE DADOS_Especies_TFG2.2_R00**
This file queries the biological occurrence database of the platform speciesLink through its API in order to collect records of plant species (*Kingdom Plantae*). The dataset is spatially filtered for the state of Rio de Janeiro, with a specific focus on the municipality of Teresópolis.
Using descriptive fields from the records (*locality*, *occurrenceRemarks*, and *habitat*), a keyword-based filtering process is applied to identify species associated with **riparian vegetation** (e.g., *mata ciliar*, riparian forest, river margins, and fluvial environments). The resulting records are processed and organized into a structured dataset and exported as a CSV file, enabling further ecological, territorial, and geospatial analyses related to vegetation associated with watercourses.

Database source: [https://specieslink.net/](https://specieslink.net/)

---

> **01_MAPAS_TFG2.2_R00.ipynb**

This notebook accesses satellite imagery and geospatial datasets through Google Earth Engine to generate base maps for the study area. The file supports the visualization and spatial analysis of environmental variables relevant to the research, such as vegetation cover, hydrography, and terrain characteristics within the municipality of Teresópolis.

---

> **02_FMP_classificação_das_casas_TFG2.2_R00**

This file contains the classification process of residential typologies within the study area based on spatial and morphological characteristics. The analysis aims to understand patterns of occupation and housing distribution in areas close to rivers and environmentally sensitive zones.

---

> **03_GEOBIAS_Zonas_de_Risco_TFG2.2_R00**

This file analyzes and maps risk zones within the territory using geospatial analysis methods. The objective is to identify areas exposed to environmental hazards, particularly those associated with flooding and proximity to watercourses.

---

> **04_GEOBIAS_SEGMENTACAO_CENARIOS_TFG2**

This file performs spatial segmentation of the territory to define different environmental and urban scenarios. The segmentation helps categorize the landscape into areas with similar physical, ecological, or urban characteristics.

---

> **05_GEOBIAS_SOLUCOES_DE_PROJETO_TFG2**

This file explores potential design strategies and spatial interventions based on the identified environmental conditions and risk zones. The objective is to propose territorial responses that consider ecological dynamics and urban vulnerability.

---

> **06_GEOBIAS_K-means_TFG2.2_R00**

This file applies the **K-means clustering** algorithm to group spatial data into clusters based on similarities in environmental and territorial variables. The clustering process supports the identification of patterns and typologies within the study area.

---

### **PREREQUISITES**

To run the scripts and notebooks, the following tools and libraries are required:

* Python 3.x
* Jupyter Notebook
* Pandas
* Requests
* Geospatial analysis libraries (e.g., GeoPandas, Earth Engine API if applicable)

---

### **INSTALLATION**

Install the required Python libraries using:

```
pip install pandas requests geopandas earthengine-api
```

---

### **VERSION**

TFG 2.2 – Revision R00

---

Se quiser, também posso **melhorar a parte do *Project Intention*** para ficar **nível TFG / artigo acadêmico** (mais forte conceitualmente para arquitetura + urbanismo + análise territorial).
