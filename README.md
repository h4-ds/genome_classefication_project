# genome_classefication_project
This project presents a comprehensive genomic data analysis pipeline aimed at studying sequence variations and mutation patterns. The project integrates bioinformatics tools for sequence alignment and preprocessing with machine learning techniques to support mutation characterization and data-driven genomic insights.

## Data Source

Raw genomic sequence data were obtained from public databases 
(e.g., NCBI / GISAID).

Due to size and privacy constraints, raw FASTA/FASTQ files are not stored in this repository.

Accession numbers will be provided upon request.



# SARS-CoV-2 Mutation Classification Project

## 1. Data Insights & Distribution
In this section, we analyze how the mutations are distributed across the dataset.

### Frequency Class Distribution

<img width="589" height="455" alt="Frequency Class Distribution" src="https://github.com/user-attachments/assets/dbb399f4-b1b2-4515-8dba-c8f93a405245" />

This plot illustrates the significant class imbalance in our dataset, where 'Rare' mutations represent the majority of the samples, followed by 'Low-frequency' and 'Common' classes.

### Conserved vs Variable Positions across the Genome

<img width="1311" height="393" alt="Conserved vs Variable Positions across the Genome" src="https://github.com/user-attachments/assets/303e3dca-ca81-427a-b47b-b2016692b3a6" />


This visualization highlights the genomic locations of mutations, comparing stable (conserved) regions versus highly mutable (variable) regions within the SARS-CoV-2 genome.

## 2. Model Performance Evaluation
Here we compare the effectiveness of **SVM** and **Random Forest** in classifying these mutations.

### Confusion Matrix Comparison

<img width="1554" height="601" alt="RF_vs_SVM_Confusion Matrix" src="https://github.com/user-attachments/assets/9e464594-d120-43e2-acc7-caf8588fa60f" />


The confusion matrices show that **Random Forest** achieved higher stability and accuracy across all classes, particularly in correctly identifying rare mutations compared to SVM.

### Decision Boundary Classification Comparison

<img width="1388" height="596" alt="Decision_Boundry_Classification_Comparison" src="https://github.com/user-attachments/assets/c2b08ff5-6ccb-47fb-9e0c-3b5ef6dc5cbe" />


This visual comparison shows how each model separates the classes based on **Allele Frequency** and **Shannon Entropy**. The Random Forest's axis-aligned partitions better capture the specific thresholds required for accurate classification.



