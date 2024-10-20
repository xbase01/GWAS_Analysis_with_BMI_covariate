GWAS Analysis with BMI Covariate
================================

Overview
--------

This repository contains the code, results, and report for a Genome-Wide Association Study (GWAS) aimed at identifying associations between genetic variants (SNPs) and a phenotype (fen4). The analysis was performed using both covariate and non-covariate models to evaluate genetic contributions to the phenotype.

The covariate used in this study was BMI (Body Mass Index), which was calculated from height and weight data. The results include detailed statistical analyses, Manhattan plots, Q-Q plots, and identification of significant SNPs, along with genotype analysis.

Files in the Repository
-----------------------

*   **GWAS.csv**: The cleaned dataset used for the analysis. It contains phenotype, covariate, and other genetic data.
    
*   **GWAS\_Analysis.ipynb**: The Jupyter Notebook that contains the entire workflow for performing GWAS, including data cleaning, visualization, model building, and SNP identification.
    
*   **GWAS\_analysis\_report.pdf**: A comprehensive report summarizing the entire study, including the study design, methodology, results, and interpretations.
    
*   **GWAS\_results\_best\_model.xlsx**: Excel file containing results from the best GWAS model (with BMI as the covariate).
    

Study Design
------------

The primary goal of this GWAS was to investigate associations between SNPs and the phenotype fen4. The study was conducted using two different models:

1.  **Without Covariate**: To evaluate direct associations between SNPs and fen4 without adjustment.
    
2.  **With Covariate (BMI)**: To control for the potential confounding effects of BMI, which was calculated from height and weight measurements.
    

### Analysis Steps

1.  **Data Preparation**: The dataset was prepared by calculating BMI as a covariate, and filtering out missing values for the variables used in the analysis.
    
2.  **Statistical Description**: Descriptive statistics and histograms were generated for fen4 and BMI to evaluate their distributions.
    
3.  **GWAS Analysis**: Two models were used, one with BMI as a covariate and one without. This was done to evaluate the potential confounding effect of BMI on SNP-phenotype associations.
    
4.  **Plot Generation**: Manhattan and Q-Q plots were created to visualize the significant SNPs and evaluate the quality of the GWAS models.
    
5.  **Identification of Significant SNPs**: From the covariate-adjusted model, the top 3 SNPs with the lowest p-values were identified and analyzed.
    

Results Summary
---------------

*   **Manhattan Plots**: Similar peaks were observed across chromosomes for both models, indicating consistent associations.
    
*   **Q-Q Plots**: Both models showed minimal inflation, with genomic inflation factors (λ GC) close to 1, indicating a reliable model fit.
    
*   **Top SNPs**: Three SNPs were identified as having the lowest p-values and were further analyzed in terms of genotype and association with fen4. No significant literature was found for these SNPs, although other information such as allele frequencies was available.
    

Key Findings
------------

*   The covariate-adjusted model with BMI was selected as the best model, as it provided a more uniform distribution of significant associations.
    
*   Three SNPs were identified with significant associations with fen4:
    
    1.  **Chr9:121775579 (rs76728852)**
        
    2.  **Chr5:85817688 (rs112244286)**
        
    3.  **Chr9:13381524 (rs10961034)**
        
*   Literature searches did not reveal any publication citations for these SNPs, but other useful data such as allele frequencies were found.
    

How to Run the Analysis
-----------------------

To replicate the analysis, follow these steps:

1.  **Clone the Repository**:
    
2.  **Install Dependencies**:Make sure you have Python 3, Jupyter Notebook, and the necessary Python packages such as hail, pandas, numpy, and seaborn installed.
    
3.  **Run the Jupyter Notebook**:Open GWAS\_Analysis.ipynb in Jupyter Notebook and run each cell sequentially to reproduce the results.
    
4.  **Request VCF File**:The .vcf file used in this analysis is not included in the repository due to its large size. It can be made available upon request.
    

Contact
-------

If you have questions or need the .vcf file, please contact Jude Aneke at \[aneke.d@phystech.edu\].

License
-------

This project is licensed under the MIT License.
