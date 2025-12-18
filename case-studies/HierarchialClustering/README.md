# Hierarchical Clustering on Customer Spend Data

This notebook demonstrates hierarchical (agglomerative) clustering on a customer spend dataset using Python. It covers data preprocessing, scaling, clustering, dendrogram visualization, and cluster interpretation.

## Overview

- **Goal:** Segment customers based on their spending attributes using hierarchical clustering.
- **Techniques:** Data cleaning, z-score normalization, pairplot visualization, agglomerative clustering (average, complete, ward linkage), dendrograms, and cophenetic correlation.
- **Libraries:** pandas, numpy, matplotlib, seaborn, scipy, scikit-learn.

## Dataset

- **File:** `Cust_Spend_Data.csv`
- **Description:** Contains customer spend data with multiple attributes. The notebook uses columns from the third onward for clustering.

## Requirements

- Python 3.7+
- pandas
- numpy
- matplotlib
- seaborn
- scipy
- scikit-learn

Install requirements with:

```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn
```

## Notebook Steps

1. **Import Libraries**
   - pandas, numpy, matplotlib, seaborn, scipy, scikit-learn.
2. **Load Data**
   - Reads `Cust_Spend_Data.csv` into a DataFrame.
   - Displays the first 10 rows.
3. **Select Attributes**
   - Selects columns from the third onward for clustering.
4. **Data Scaling**
   - Applies z-score normalization to each attribute.
5. **Visualization**
   - Uses seaborn's `pairplot` to visualize attribute distributions and relationships.
6. **Agglomerative Clustering**
   - Performs clustering with 3 clusters using average linkage and Euclidean distance.
   - Assigns cluster labels to each customer.
7. **Cluster Analysis**
   - Groups data by cluster labels and computes mean attribute values for each cluster.
8. **Dendrograms and Cophenetic Correlation**
   - Computes linkage matrices for average, complete, and ward methods.
   - Calculates cophenetic correlation to assess clustering quality.
   - Plots dendrograms for each linkage method.

## Key Outputs

- Pairplot of scaled attributes.
- Cluster labels for each customer.
- Mean attribute values per cluster.
- Dendrograms for different linkage methods.
- Cophenetic correlation coefficients.

## How to Run

1. Place `Cust_Spend_Data.csv` in the same directory as the notebook.
2. Install required libraries.
3. Open the notebook in Jupyter and run all cells.

## Interpretation

- The notebook helps identify natural groupings among customers based on their spending patterns.
- Dendrograms and cophenetic correlation provide insight into the quality and structure of the clusters.

## References

- [scikit-learn Agglomerative Clustering](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html)
- [scipy.cluster.hierarchy](https://docs.scipy.org/doc/scipy/reference/cluster.hierarchy.html)
- [Seaborn Pairplot](https://seaborn.pydata.org/generated/seaborn.pairplot.html)
