# BCB546X_FinalGroup
This repository holds the materials for the completion for The Eclectics group project for BCB546X. 

Our goal was to recreate the findings from Leininger et al. 2014 (see .pdf within).

Within the base repository you will find the following files:
  1. Weeger_et_al2019.md : This introduces the original paper, explaining the technical details of our replication of analyses and summarizes our results from our attempts. 
  2. Jupyter file : Contains the commented work flow code for our replication. 
  3. Presentation.pptx : The presentation associated with this repository. 
  4. Leininger_et_al2014.pdf : The paper we used to base this report on. 
  
The main directories are as follows 
  1. **Data_raw** contains the original files we used, as well as the scripts used to obtain the larger fastq files that could not be stored here. 
  2. **Figure_heatmap** contains all files generated during the heatmap analysis. This includes the code used in RSEM, the R code for DESeq, all intermediary files and result files. 
  3. **Figure_PhyloTree** contains all files generated during the phylogenetic tree analysis. This includes all intermediary files, as well as results. 
  
 Within **Figure_heatmap**, you will find the following content:
   * **_individual_** folder: read counts results from RSEM, includes 33 files from each replications of each developmental stages generated by *Ryan Fortune*.
  * **_BCB546X_FinalGroup.Rproj_**: R project of differential expressed gene analysis and heatmap.
  * **_RNAseq_GeneExpression_** folder: includes code, metadata and results of differential expressed gene analysis and heatmap.
      * **final.Rmd_**: the workflow and code.
      * metadata:
          * **_genes.csv_**: list of gene names and their sequence ID.
          * **_samples_**: list of read counts result file names and their developmental stages.
      * results of significantly differential expressed gene in apical region:
          * **_DEG top_bottom.csv_**: DE genes between the top and bottom part.
          * **_DEG top_middle.csv_**: DE genes between the top and middle part.
      * **_heatmap.jpg_**: heatmap of gene expression level in all developmental stages.

Within **Figure_PhyloTree**, you will find the following content:
  * All files generated by MrBayes. 

  
[Created and edited by E. Glynne, A. Weeger, R. Fortune, H. Liu, A. Anilkumar ]
