# Character N-gram Language Identification

A Natural Language Processing project for **English–Turkish language identification** using character-based **2-gram** and **3-gram** language models.

The project builds character n-gram models with **Laplace smoothing**, evaluates them using **10-fold cross-validation**, compares their performance with standard classification metrics, and performs statistical significance and out-of-vocabulary (OOV) analysis.

## Overview

Character n-grams are useful for language identification because they capture language-specific patterns such as:

- Letter combinations
- Diacritics
- Character sequences
- Writing patterns

This project compares 2-gram and 3-gram models for distinguishing English and Turkish sentences.

## Features

- PDF and DOCX text extraction
- Text preprocessing and sentence splitting
- Character-based 2-gram language model
- Character-based 3-gram language model
- Laplace (add-one) smoothing
- English–Turkish sentence classification
- 10-fold cross-validation
- Accuracy, precision, recall, and F1-score evaluation
- Out-of-vocabulary (OOV) testing
- Paired t-test for statistical significance
- Additional error and mixed-language analysis

## Results

The models were evaluated using 10-fold cross-validation.

| Model | Mean Accuracy | Mean F1-score |
|---|---:|---:|
| 2-gram | 83.75% | 83.60% |
| 3-gram | 88.29% | 88.19% |

The 3-gram model achieved higher overall performance than the 2-gram model.

A paired t-test was also used to compare model performance across the folds. The reported p-values were below 0.05 for accuracy, precision, recall, and F1-score, indicating a statistically significant difference between the two models.

## Dataset

Two corpora were used:

- English corpus
- Turkish corpus

The notebook extracts and preprocesses text from uploaded documents before splitting the data into sentences.

Corpus source files are not included in this repository.

## Technologies

- Python
- NLTK
- NumPy
- Pandas
- scikit-learn
- SciPy
- Matplotlib
- Seaborn
- PyPDF2
- python-docx
- Jupyter / Google Colab

## Project Structure

```text
character-ngram-language-identification/
│
├── language_identification.ipynb
├── requirements.txt
└── README.md
