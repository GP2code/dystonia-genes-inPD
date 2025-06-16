# Hidden Connections? Assessing Dystonia Gene Variants in Parkinson’s Disease

<div align="center">
    <a href="https://gp2.org/">
    <img src="https://www.michaeljfox.org/sites/default/files/styles/grant_image_opportunity_detail/public/grant/GP2%20Logo.png?itok=OhZkYS-H" alt="GP2 Logo" width="200">
</a>
</div>


`GP2 ❤️ Open Science 😍`
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![DOI](https://zenodo.org/badge/1003012684.svg)](https://doi.org/10.5281/zenodo.15676002)


**Last Updated:** June 2025

## Summary
This repository contains the code and workflow used in the study:
**“Hidden Connections? Assessing Dystonia Gene Variants in Parkinson’s Disease”.**

In this analysis, we screened whole-genome sequencing (WGS) data from the GP2 Release 8 dataset for rare pathogenic/likely pathogenic variants in 28 dystonia-linked genes across 15,739 individuals (7,852 PD, 4,287 atypical parkinsonism, and 3,600 controls).

The core notebook provided here demonstrates how we extracted variant carriers and performed initial annotation across multiple ancestries using plink, bcftools, and annovar, followed by BigQuery-based downstream analysis.

Summary statistics and full results are available through GP2 Tier 1 and AMP-PD approved data platforms.

## Data Statement
* The data was obtained from the Global Parkinson’s Genetics Program (GP2) release 8 (GP2 release 8, DOI: 10.5281/zenodo.13755496) and access can be requested through the Accelerating Medicines Partnership in Parkinson’s Disease (AMP-PD) via the online application process (https://www.amp-pd.org/)
* AMP-PD Release 4 (https://www.amp-pd.org/)
    * Access to these data requires approval through the AMP-PD platform

## Citation
If you use this repository or find it helpful for your research, please cite the corresponding manuscript:

>Hidden Connections? Assessing Dystonia Gene Variants in Parkinson’s Disease
>
>Lange LM, Fang ZH, Screven L, Tan AH, et al.,
>
>Global Parkinson’s Genetics Program (GP2), 2025
[pending]

### Helpful Links 
- [GP2 Website](https://gp2.org/)
    - [GP2 Cohort Dashboard](https://gp2.org/cohort-dashboard-advanced/)
- [Introduction to GP2](https://movementdisorders.onlinelibrary.wiley.com/doi/10.1002/mds.28494)
    - [Other GP2 Manuscripts (PubMed)](https://pubmed.ncbi.nlm.nih.gov/?term=%22global+parkinson%27s+genetics+program%22)

## Repository Orientation
The `analyses/` directory includes all the analyses discussed in the manuscript or links to the respective GitHubs where analyses were followed.
```
├── analyses/
│   └── GP2_WGS_data_dystonia.ipynb
├── LICENSE
└── README.md
```

## Analyses
| **Notebook**                   | **Description**                                                                                                                                                         |
| ------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| GP2\_WGS\_data\_dystonia.ipynb | Extracts rare pathogenic variants in dystonia-linked genes across ancestries using GP2 WGS data, and generates lists of variant carriers for downstream interpretation. |

## Software
| **Software**    | **Version(s)** | **Resource URL**                                                                                       | **Notes**                                                      |
| --------------- | -------------- | ------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------- |
| Python          | 3.8+           | [http://www.python.org/](http://www.python.org/)                                                       | Used for downstream analysis and scripting.                    |
| PLINK           | 1.9 / 2.0      | [http://www.cog-genomics.org/plink/](http://www.cog-genomics.org/plink/)                               | Used for variant filtering and extraction.                     |
| BCFtools        | 1.17+          | [http://www.htslib.org/](http://www.htslib.org/)                                                       | Used for variant extraction.                                   |
| ANNOVAR         | Latest         | [https://annovar.openbioinformatics.org/en/latest/](https://annovar.openbioinformatics.org/en/latest/) | Used for variant annotation.                                   |
| Google BigQuery | -              | [https://cloud.google.com/bigquery](https://cloud.google.com/bigquery)                                 | Used for querying GP2 metadata and integrating phenotype data. |

## Disclaimer
This notebook accompanies the manuscript Hidden Connections? Assessing Dystonia Gene Variants in Parkinson’s Disease and is intended to facilitate transparency and reproducibility of the variant extraction and annotation workflow.
