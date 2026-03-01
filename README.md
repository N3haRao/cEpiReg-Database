# 🧬 cEpiReg-Database

**Context-Specific Epigenetic Regulatory Network Database for Alzheimer’s Disease**

---

## Live Demo

**Database Website:**
[https://bioed.bu.edu/students_24/Team_10/Team-10_database.html](https://bioed.bu.edu/students_24/Team_10/Team-10_database.html)

**Project Overview Video:**
Available on the homepage of the live site.

> ⚠️ Note: This repository contains the source code used for the Boston University deployment.
> Some asset paths are configured for the BU course server environment.

---

## Project Summary

**cEpiReg** constructs a comprehensive database elucidating the intricate regulatory mechanisms underlying Alzheimer's Disease (AD) genetics.

By integrating:

* **Single-cell RNA-seq (scRNA-seq)**
* **Single-cell ATAC-seq (scATAC-seq)**
* **eQTL analysis**
* Public databases (ENCODE, Epimap, GWAS Catalog, UCSC, dbSNP)

we identified and connected:

* Transcription Factors (TFs)
* Target Genes (TGs)
* Cis-Regulatory Elements (CREs)
* Disease-associated SNPs

This project establishes a regulatory framework linking **TF → CRE → Target Gene → Genetic Variant**, uncovering hidden regulatory relationships critical for understanding AD pathogenesis.

Done in collaboration with the [Hou Lab](https://hougroup.xyz/).

---

## Methods Overview

The cEpiReg framework integrates multiple analytical pipelines:

### Gene Regulatory Network Construction

* Built GRNs using **pySCENIC**
* Identified transcription factor → target gene relationships

### CRE Identification (ATAC-seq)

* Linked cis-regulatory elements to genes
* Cross-referenced with ENCODE and Epimap datasets

### eQTL Integration

* Associated SNPs with genes and CREs
* Connected regulatory variation to disease genetics

### Web-Based Database Implementation

* Interactive query interface
* Downloadable data tables (.csv, .txt)
* External database linking (UCSC, dbSNP)
* Network visualizations (NetworkX + Plotly)
* Integrated help documentation

While full multi-layer integration was limited by cell-type and tissue-specific sample constraints, the platform successfully integrates independent regulatory modules into a cohesive database interface.

---

## Key Features

* Gene and region query functionality
* Interactive network visualizations
* Downloadable query results (.csv / .txt)
* External database integration (UCSC Genome Browser, dbSNP)
* Heatmaps and CRE visualizations
* Structured navigation across GRN, CRE Explorer, and eQTL modules
* Comprehensive help page

---

## Repository Contents

| File                            | Description                    |
| ------------------------------- | ------------------------------ |
| `Team-10_database.html`         | Homepage                       |
| `GRN-test.html` / `grn-test.py` | Gene Regulatory Network module |
| `ATAC.html` / `ATAC_AJAX.py`    | CRE Explorer module            |
| `eQTL-data.html` / `eqtl.py`    | CRE + eQTL integration module  |
| `styles.css` / `style1.css`     | Website styling                |
| `Database_Overview.mp4`         | Demo video                     |
| `NR-biorender-cepireg-logo.png` | Project logo                   |

---

## Team Contributions

### Neha Rao

* Designed homepage, navigation UI, and Help page
* Developed GRN query system and visualizations
* Implemented interactive networks using **NetworkX + Plotly**
* Enabled downloadable visualizations (.png) and tables (.csv)

### Jawahar Mahendran

* Designed CRE Explorer module
* Implemented Pie Charts, Data Tables, and IGV integration
* Enabled .txt download functionality
* Contributed to Help page revisions

### Bhavana Kapalli

* Designed CRE + eQTL module
* Integrated UCSC/dbSNP external links
* Implemented Google Charts heatmap visualization
* Enabled downloadable .csv outputs
* Help page design contributions

---

## Conference Proceedings / Abstracts Resulting from This Work

**Fu, T. T., Mahendran, J., Kapalli, B., Rao, N., Farrer, L., & Hou, L. (2025).**
*W50. Epigenetic regulatory network in microglia reveals context-dependent trans-regulatory programs in brain disease.*
European Neuropsychopharmacology, 99, 234.

**Fu, T. T., Kapalli, B., Mahendran, J., Rao, N., & Hou, L. (2024).**
*Leveraging context-specific epigenomic regulatory networks (EPINETS) to dissect the genetics of neuropsychiatric disorders.*
European Neuropsychopharmacology, 87, 8.

---

## Acknowledgments

We extend our heartfelt gratitude to:

* **Dr. Lei Hou**
* **Dr. Ting-Ting Fu**

for their mentorship, guidance, and expertise throughout the development of the cEpiReg-Database.

The database was developed at Boston University as part of the BF768 course (Spring 2024).

---

## Technologies Used

* Python
* pySCENIC
* NetworkX
* Plotly (JavaScript)
* Google Charts
* HTML / CSS
* AJAX
* UCSC Genome Browser integration

