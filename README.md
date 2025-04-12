# 🧬 Assignment 4 — PWM-Based Transcription Factor Binding Site Analysis

**👩‍💻 Author:** Tejaswini Repala  
**📅 Date:** February 12, 2024  
**💻 Language:** Python 3.11.4  

---

## 📖 Description

This project identifies potential **transcription factor binding sites** for **ArgR** in *Escherichia coli K12* by constructing a **Position Weight Matrix (PWM)** from a nucleotide counts matrix.

The analysis follows these steps:
- Constructs a PWM from the counts matrix (with pseudocounts to avoid log(0))
- Normalizes to frequency and calculates log2-based scores
- Scans upstream regulatory regions of genes using a sliding window
- Outputs the **top 30 gene IDs** with the highest PWM similarity scores — potential ArgR binding sites

---

## 📦 Dependencies

Install dependencies using:

```bash
pip install numpy pandas

    
### Input:
argR-counts-matrix.txt

E_coli_K12_MG1655.400_50

### Output Files:

The script prints to the console the top 30 gene IDs with the highest PWM scores, indicating the potential binding sites for the argR transcription factor.
