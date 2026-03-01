# cEpiReg-Database

cEpiReg constructs a comprehensive database elucidating the intricate regulatory mechanisms underlying Alzheimer's Disease (AD) genetics. Through integrating data from scRNA seq and sc-ATAC seq, we identified the cis-regulatory elements (CREs) by comparing our results against various databases like ENCODE, Epimap, GWAS Catalog, and publicly available datasets. This project establishes a robust framework connecting transcription factors (TFs), CREs, and target genes. cEpiReg uncovers hidden regulatory links that could piece together missing links crucial for understanding AD pathogenesis.

Done in collaboration with the [Hou Lab](https://hougroup.xyz/). 

## Accomplishments
Our team tackled a multifaceted project on the gene regulatory landscape in Alzheimer's Disease (AD). We constructed gene regulatory networks (GRNs) and linked transcription factors (TFs) to target genes
(TGs) using pySCENIC, and established connections between cis regulatory elements (CREs) and TGs through ATACseq analysis. Leveraging eQTL analysis, we associated SNPs with genes and their CREs, enhancing our understanding of the CRE landscape. These insights were integrated into a user-friendly web interface at https://bioed.bu.edu/students_24/Team_10/Team-10_database.html. While we aimed to merge these analyses to infer the entire genetic landscape for AD, constraints in sample data, particularly cell-type and tissue-type specificity, prevented full integration. However, our team successfully implemented database integration, user interface development, data query functionalities, data download features, external database linkage, and creation of a comprehensive help page, resulting in a robust platform for navigating AD-related regulatory networks.

## Limitations and Difficulties
Integrating Google Charts for visualization posed challenges, necessitating extensive trial and error to align data outputs with chart inputs. Distinguishing between Python, HTML, and AJAX errors added complexity to debugging, mitigated by leveraging console.log statements and "Inspect" functions. Furthermore, managing large file sizes impeded data loading on the website.

## Team Contributions
- Neha Rao (33.3%): Designed the user interface (UI), queries and visualizations for the Gene Regulatory Network page. Developed interactive network visualizations using NetworkX and Plotly JavaScript, enabling users to download visualizations as .png files. The query results (tables) can be downloaded as .csv files. Also, spearheaded the design and implementation of the homepage, menu UI, and the Help page.
- Jawahar Mahendran (33.3%): Designed the CRE Explorer page. Implemented diverse viewing options such as Pie Charts and Data Tables, alongside the functionality to query genes and chromosome regions using IGV. Integrated a data download feature for the results in .txt format. Assisted with Help page modification.
- Bhavana Kapalli (33.3%): CRE & eQTL page UI design and implementation and related query design, and implementation. Links for output in data table to UCSC/dbSNP. Heatmap using google charts, a menu driven selection of data and data download into a file (.csv). Help page design.

## Acknowledgments
We extend our heartfelt gratitude to Dr. Lei Hou and Dr. Ting-Ting Fu for their unwavering support, guidance, and mentorship throughout this project. Their expertise and insights have been invaluable in the development of the cEpiReg-Database.
