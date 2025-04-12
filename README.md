### Title: Assignment4

### Author: Tejaswini Repala

### Date: February 12, 2024

### Programming Language & Version: Python 3.11.4

### Description:

This script performs transcription factor binding site identification using a Position Weight Matrix (PWM) derived from a counts matrix for a specific transcription factor known as argR. The script calculates the PWM from the provided counts matrix by augmenting counts to avoid zero values and then uses this matrix to scan the upstream regulatory regions of genes in the Escherichia coli K12 genome. The analysis identifies potential binding sites by comparing gene sequences to the PWM and outputs the top 30 gene IDs with the highest similarity scores, suggesting these regions as potential targets for argR binding.

### Dependencies:

NumPy: For numerical operations including matrix calculations.

Pandas: For data handling and DataFrame manipulation.

These dependencies can be installed using the following command:

    pip install numpy pandas
    
### Input:
argR-counts-matrix.txt

E_coli_K12_MG1655.400_50

### Output Files:

The script prints to the console the top 30 gene IDs with the highest PWM scores, indicating the potential binding sites for the argR transcription factor.
