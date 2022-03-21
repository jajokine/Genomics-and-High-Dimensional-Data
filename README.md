## Genomics-and-High-Dimensional-Data

# MITx - MicroMasters Program on Statistics and Data Science - Data Analysis: Statistical Modeling and Computation in Applications - Second Project

The second project of the MIT MicroMasters Program course on Data Analysis analyzed a single-cell RNA-seq dataset, with the goal of unveiling
hierarchical structure and discovering important genes from it. To be more precise, the challenge was to find ways to extract meaningful information from a high-dimensional dataset compiled by the Allen Institute that contains cells from the mouse neocortex, a region in the brain which governs higher-level functions such as perception and cognition.

The larger p2_unsupervised set consists of 2,169 rows, depecting cells, and 45,768 columns, depecting genes, corresponding to the normalized transcript compatibility count (TCC) of an equivalence class of short RNA sequences, rescaled to units of counts per million. Unfortunately, the datasets themselves are too large to be downloaded to GitHub, as even the reduced set is over 300MB. However, some similar (but smaller) datasets can be found from the Allen Institute (https://portal.brain-map.org/atlases-and-data/rnaseq).

The data was first analyzed with different dimensionality reduction and data visualization techniques such as Principal Components Analysis (PCA), Multidimensional Scaling (MDS), and t-Distributed Stochastic Neighbor Embedding (t-SNE), together with some unsupervised learning techniques for clustering data, such as Hierarchical Clustering and K-Means Clustering. The clustering was then combined with logistic regression in order to distinguish informative features to be used to distinguish cells of different types. Additional smaller datasets p1, p2_evaluation and the reduced versions of p2 were also provided to help with the analysis. The statistical application of the different methods and the code for the project was made with Jupyter Notebook which also includes analysis from the written report that was part of the projet.


## Dataset

  - p1: The folder contains a small, subset of the data. It contains count matrix **X** along with "ground truth" clustering labels _y_, which were obtained
  by scientists using domain knowledge and statistical testing (511 by 45768 matrix for X and 511 by 1 matrix for y).
  - p2_unsupervised: The folder contains only a count matrix (2169 by 45768 matrix for X and 2169 by 1 matrix for y).
  - p2_evualation: The folder contains a labeled training (1077 by 45768 matrix for X and 1077 by 1 matrix for y) and test set (1108 by 45768 matrix for X and 1108 by 1 matrix for y). 
  - p2_unsupervised_reduced and p2_evaluation_reduced: These folders contain datasets with a reduced number of genes (2169 by 20000 training matrix for X and 2169 by 1 training matrix for y, 1077 by 20000 training evaluation matrix for X and 1077 by 1 training evaluation matrix for y, and 1108 by 20000 testing evaluation matrix for X and 1108 by 1 testing evaluation matrix for y).
 
## Access and Requirements

The file [project2.ipynb](https://github.com/jajokine/Genomics-and-High-Dimensional-Data/blob/main/project2.ipynb) is the Jupyter Notebook that contains all the code, visualizations and analysis of the project.

The dependencies and requirements can be seen from requirements.txt that can be installed in shell with the command:

      pip install -r requirements.txt
  
