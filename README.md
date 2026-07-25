Overview


This repository contains an automated RNA-seq bioinformatics pipeline designed to distinguish Long COVID (PASC) patients from recovered convalescent controls using PBMC gene expression signatures (GEO Accession: GSE226260). The pipeline integrates data retrieval, quality control, differential expression testing (DESeq2), and supervised machine learning (randomForest / caret) to evaluate diagnostic biomarkers.


Setup


1. Create environment from yml file via bash command:
  conda env create -f environment.yml


2. Activate environment via bash command:
  conda activate RIBF125-final


Usage


3. To render the complete HTML report and execute all statistical/ML steps 
  from the command line, run:


  Rscript -e "rmarkdown::render('RBIF125_Final_Prior.Rmd', output_format = 'html_document')"


Output


The resulting html file from the Rmarkdown script will be generated in the current directory. All figures, metrics, and tabular outputs will automatically be saved to results/figures/ 
and results/tables/ in the current directory where the RBIF125_Final_Prior.Rmd file is located.