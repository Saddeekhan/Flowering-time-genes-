**Flowering Time Gene Expression Analysis**

This repository contains a Python script for analyzing and visualizing flowering time gene expression data from RNA-seq experiments. The workflow includes data preprocessing, normalization, clustering, and visualization of gene expression patterns across developmental stages.

**Features**

The script performs the following steps:

**1. Import Libraries**

Uses pandas for data handling, numpy for numerical operations, matplotlib and seaborn for visualization, and scikit-learn for preprocessing and clustering.

**2. Load Data**

Reads gene expression data (genes.fpkm_tracking) into a Pandas DataFrame.

**3. Select Expression Data**

Extracts the gene_id column and FPKM values across developmental stages (M1–M8).

**4. Handle Missing Values**

Uses SimpleImputer with the median strategy to replace missing values in the dataset.

**5. Normalize Data**

Standardizes FPKM values using StandardScaler (mean = 0, standard deviation = 1).

**6. Summarize Expression Profiles**

Computes mean normalized FPKM values across all stages.

**7. Data Visualization**

I. KDE plot of mean normalized expression values.

II. Line plot showing mean expression across stages.

III. Scatter plot of normalized values.

**8. Focus on Flowering Time Genes**

Defines a list of genes of interest related to flowering time.

Filters the dataset to extract and visualize their expression patterns.

**9. Expression Profile Plot**

Generates a line plot of flowering time gene expression across stages M1–M8, including markers, labels, and legends for clear interpretation.

**Example Plots**

I. KDE plot of normalized FPKM distribution

II. Line plot of mean gene expression across stages

III. Expression profile plot of selected flowering time genes

**Requirements**

1. Python 3.x

2. pandas

3. numpy

4. matplotlib

5. seaborn

6. scikit-learn

**Install dependencies with:**

pip install -r requirements.txt

**Usage**

Place your genes.fpkm_tracking file in the working directory.

Update the list of genes_of_interest in the script.

**Run the script:**

python flowering_time_analysis.py


View the generated plots for insights into flowering time gene expression patterns.

**Summary**

This project provides a reproducible pipeline to:

Clean and normalize RNA-seq expression data

Explore global expression trends

Visualize specific gene expression profiles across developmental stages

It can be easily adapted to study other gene sets or biological processes.
