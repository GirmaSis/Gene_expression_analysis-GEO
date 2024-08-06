# Gene expression analysis: 
## [PCA, clustering and feature interpretation]

## Overview
This project demonstrates a comprehensive analysis of gene expression data using Principal Component Analysis (PCA), clustering, and feature interpretation techniques. The dataset used in this project is sourced from the GEO database. 

## Dataset
The gene expression dataset with an accession number [GSE12345](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE12345) consists of gene expression profiles of human pleural mesotheliomas samples.

> **Objective:** to utilize PCA to reduce the dimensionality of the dataset, perform clustering to group similar samples, and interpret the features that contribute most to the principal components. This helps to provide insights into the gene expression profiles.

## Steps followed

### 1. Data preprocessing
- **Technique**: Standardization
- **Description**: The gene expression data is loaded and standardized to ensure that each feature contributes equally to the analysis.

### 2. Dimensionality reduction using PCA
- **Algorithm**: Principal Component Analysis (PCA)
- **Description**: PCA is applied to reduce the dimensionality of the dataset. The explained variance ratio and cumulative explained variance are calculated to determine the number of principal components needed. 
```bash
variance_threshold = 0.95
Number of components to retain 95.0% of variance: 11
```

### 3. Clustering of transformed data
- **Algorithm**: KMeans Clustering
- **Description**: KMeans clustering is applied to the reduced-dimension data obtained from PCA. 

### 4. Feature interpretation
- **Technique**: Analysis of PCA Loadings
- **Description**: The principal components are interpreted by identifying the top contributing genes. This helps in understanding which genes contribute most to the variability captured by each principal component.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Gene_expression_analysis-GEO.git
   cd Gene_expression_analysis-GEO


