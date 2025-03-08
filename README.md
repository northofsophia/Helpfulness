# Measuring the Helpfulness of AI Generated Text

## Overview
This repository contains code and data for analyzing the helpfulness of AI-generated text in creative writing. Our goal is to develop automatic metrics that assess helpfulness.

Helpfulness in this context is defined as the likelihood of a user accepting or rejecting an AI-generated suggestion. We investigate three key aspects of helpfulness:
- **Coherence**: How well the AI-generated text integrates into the existing writing.
- **Creativity**: The originality and inventiveness of the suggestion.
- **Stylistic Fit**: The alignment of tone and lexical structure with the user's writing.

## Repository Structure
This repository contains code and data for analyzing the helpfulness of specific metrics related to stylistic fit, coherence, and creativity. The structure is as follows:

`Code` - Contains Jupyter notebooks for calculating and analyzing helpfulness metrics.


`Data` - Contains CSV files with collected and processed data for further analysis.

## Usage
*  **Running the Notebook**: Open `.ipynb` notebook and execute the cells to generate and analyze data.

*  **Using the Data**: The final results are stored in `Data/all_metrics_upd.csv`, which contains combined scores for coherence, creativity, and stylistic fit. This file can be used for further statistical analysis or model training.

## Metrics
We assess metrics for three different aspects of helpfulness: coherence, creativity, and stylistic fit. There are three notebooks that go into detail on how to calculate each of these metrics using the [CoAuthor](https://coauthor.stanford.edu/) data. They are `Detecting_Stylistic_Fit_(TONE_and_POS)_Prompt_vs_Suggestions.ipynb`, `creativity.ipynb`, and `Coherence_Scores.ipynb`. 

Lastly, we combine all the metrics into a final csv `all_metrics_upd.csv` using code from `ALL_Metrics.ipynb`

## Getting Weights
To get individual weights for any workerID, use `all_metrics_upd.csv` and `weightedSum.ipynb`. Once you have the csv, execute the cells in `weightedSum.ipynb` to compute the weight metrics.
