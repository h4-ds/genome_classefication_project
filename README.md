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
![Frequency Class Distribution](Freque<img width="589" height="455" alt="Frequency Class Distribution" src="https://github.com/user-attachments/assets/d4692c8f-02ac-4345-80d0-6cd04b40caba" />
ncy_Class_Distribution.png)
* **Description:** This plot illustrates the significant class imbalance in our dataset, where 'Rare' mutations represent the majority of the samples, followed by 'Low-frequency' and 'Common' classes.

### Conserved vs Variable Positions across the Genome
![Conserved vs Variable Positions](Conserved_vs_Variable_Positions_across_the_Genome.png)
* **Description:** This visualization highlights the genomic locations of mutations, comparing stable (conserved) regions versus highly mutable (variable) regions within the SARS-CoV-2 genome.

## 2. Model Performance Evaluation
Here we compare the effectiveness of **SVM** and **Random Forest** in classifying these mutations.

### Confusion Matrix Comparison
![Confusion Matrix](RF_vs_SVM_Confusion_Matrix.png)
* **Description:** The confusion matrices show that **Random Forest** achieved higher stability and accuracy across all classes, particularly in correctly identifying rare mutations compared to SVM.

### Decision Boundary Classification Comparison
![Decision Boundary](Decision_Boundry_Classification_Comparison.png)
* **Description:** This visual comparison shows how each model separates the classes based on **Allele Frequency** and **Shannon Entropy**. The Random Forest's axis-aligned partitions better capture the specific thresholds required for accurate classification.



