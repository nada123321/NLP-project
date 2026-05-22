# Prompting and Complexity Modeling for Text-to-Cypher Generation

This repository contains the material for an NLP homework project on Text-to-Cypher generation and Cypher query complexity classification.

## Project Overview

The project has two main components:

1. **Text-to-Cypher generation with Qwen**
   - comparison of four prompting strategies
   - evaluation on a reduced benchmark of 30 natural-language questions
   - final evaluation based on Neo4j execution and output comparison with gold queries

2. **Cypher difficulty classification**
   - supervised baseline for predicting Cypher query difficulty levels
   - TF-IDF representation with an MLP trained from scratch

## Main Files

- `prompt1_qwen_dataset30_colab.ipynb`  
  Direct schema-aware prompting baseline.

- `prompt2_qwen_dataset30_colab.ipynb`  
  Task-splitting prompting strategy.

- `prompt3_qwen_dataset30_colab.ipynb`  
  Iterative refinement prompting strategy.

- `prompt4_qwen_dataset30_colab.ipynb`  
  Hybrid prompting strategy proposed after the initial evaluation.

- `cypher_difficulty_classification_baseline.ipynb`  
  Supervised Cypher difficulty classification baseline.

- `final_report_text2cypher.md`  
  Final written report for the project.

## Dataset

The generation experiments use a reduced dataset of 30 queries (`dataset_30.csv`).  
The Colab notebooks are configured to download this dataset directly from Google Drive.

The classification experiment uses:
- `combined_text2cypher.csv`
- `curated_2500.csv`

## Evaluation

For the generation task, notebook result files store generated Cypher strings, parsing information, and exact-match indicators.  
However, the final performance figures reported in the project are based on **manual Neo4j execution and output comparison** against the gold queries.

## Author

Nada Bou Kanaan
