# Genomics-and-High-Dimensional-Data
MITx - MicroMasters Program on Statistics and Data Science - Data Analysis: Statistical Modeling and Computation in Applications - Second Project

The second project of the MIT MicroMasters Program course on Data Analysis analyzed a single-cell RNA-seq dataset, with the goal of unveiling
hierarchical structure and discovering important genes. To be more precise, the challenge was to find ways to extract meaningful information from a high-dimensional dataset compiled by the Allen Institute that contains cells from the mouse neocortex, a region in the brain which governs higher-level functions such as perception and cognition.

The larger p2_unsupervised set consists of 2169 rows and 45,768 columns which was to be analyzed with different visualization and unsupervised learning techniques with the help of smaller datasets 


**DATASET**

  - p1: The folder contains a small, subset of the data. It contains count matrix **X** along with "ground truth" clustering labels _y_, which were obtained
  by scientists using domain knowledge and statistical testing.
  - p2_unsupervised: The folder contains only a count matrix.
  - p2_evualation: The folder contains a labeled training and test set. 
  - p2_unsupervised_reduced and p2_evaluation_reduced: These folders contain datasets with a reduced number of genes.
 
Unfortunately the datasets are too large to be downloaded to GitHub, as even the reduced set is over 300MB. However, some similar datasets can be found from the Allen Institute (https://portal.brain-map.org/atlases-and-data/rnaseq). 

The statistical application of methods and code for the project is made with Jupyter Notebook and the written report is a pdf-file.
  
