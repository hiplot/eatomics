# Eatomics
Eatomics is a web application developed using Shiny. Eatomics enables fast exploration of differential expression and pathway analysis to researchers with limited bioinformatics knowledge.The application will aid in quality control of the quantitative proteomics data, visualization, differential expression and pathway analysis. Highlights of the application are an extensive experimental setup module, the data and report generation feature and the multiple ways to interact and customize the analysis. 

# Getting started

## Input Files
1. The proteinGroups.txt (e.g. txt files) as generated by the quantitative analysis software of raw mass spectrometry data - MaxQuant. The file should contain at least the columns Protein IDs, Majority protein IDs, Gene names, LFQ/iBAQ measurement columns, Reverse, Potential contaminant, Only identified by site. The latter three may be empty.
2. The sample description file - a tab separated .txt input m x n matrix file containing the clinical/observational/experimantal details of m number of patients with n number of parameters.

# Troubleshooting 

R version < 3.6 will need a lower version of caTools in order to create proper reports from rmarkdown - this might help to fix any caTools related errors.
install.packages("https://cran.r-project.org/src/contrib/Archive/caTools/caTools_1.14.tar.gz", repos=NULL, type="source")
