# Predicting-essential-genes-in-Cryptococcus-neoformans-using-metabolic-modeling-and-machine-learning

This project uses metabolic modeling and machine learning to predict essential genes in the fungal pathogen *Cryptococcus neoformans*. Essential genes are those whose deletion prevents cellular growth and they are important candidates for antifungal drug targets.

## Project Overview

- Load the iCryptococcus metabolic model using COBRApy  
- Simulate single-gene knockouts across multiple nutrient environments  
- Build metabolic graphs (reaction-sharing and metabolite adjacency)  
- Extract graph centrality features (degree, betweenness, closeness)  
- Combine simulation outputs and graph features into a machine learning dataset  
- Train models to classify genes as **essential** vs **non-essential**

## Files

- `cryptococcus_essential_genes.ipynb`  
  Main notebook containing:
  - Data loading and preprocessing  
  - Flux balance analysis (FBA) simulations  
  - Graph construction and feature extraction  
  - Model training, evaluation, and visualizations  

(If applicable)
- `data/` – input model files or metadata (not included here due to size; see notes below).
- `figures/` – selected result plots used in the report.

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/cryptococcus-essential-genes.git
   cd cryptococcus-essential-genes
