# Bangla Text Summarizer

A text summarization tool designed specifically for the Bengali language, enabling users to generate concise summaries of Bengali text documents. This project explores deep learning approaches to address the challenge of information overload by automating content condensation.

## Features

* **On-Demand Summarization**: Generate summaries from Bengali text inputs quickly and accurately.
* **Bengali Language Support**: Tailored preprocessing and modeling for Bengali, including a custom stopword list (stopwords-bn.txt).
* **Deep Learning Approach**:
   * Primary summarization using a pre-trained deep learning model (summary_model.pkl).
   * Advanced experimental summarization capabilities (see DL_summarizer.ipynb).
* **Flexible Workflows**: Supports both end-user summarization and model training/evaluation.

## Purpose

The Bangla Text Summarizer aims to help users—such as readers, analysts, or content curators—quickly grasp the main ideas of Bengali articles, reports, or documents without reading them in full. It tackles the problem of information overload by providing automated, language-specific summarization.

## Getting Started

### Prerequisites

* Jupyter Notebook environment
* Python 3.8+
* Libraries: pandas, scikit-learn, nltk, tensorflow or pytorch, transformers

### Usage

* **Summarize Text**:
   * Use the notebooks to load the pre-trained deep learning model (summary_model.pkl) for summarization.
   * Example code is provided within the notebooks.

* **Train a Model**:
   * Use BENSUMM.ipynb and DL_summarizer.ipynb for model training and experimentation.
   * Provide training data in .csv format (e.g., bensumm_data.csv).

## Repository Structure

* BENSUMM.ipynb: Notebook for summarization development, training, and inference.
* DL_summarizer.ipynb: Notebook for additional deep learning-based summarization experiments.
* summary_model.pkl: Pre-trained deep learning summarization model.
* stopwords-bn.txt: List of Bengali stopwords for preprocessing.
* bensumm_data.csv, data.csv, final_data.csv: Datasets for training and evaluation.

## How It Works

1. **Input**: Bengali text (e.g., articles, reports).
2. **Preprocessing**: Text cleaning and stopword removal using stopwords-bn.txt.
3. **Summarization**:
   * Deep Learning: Generates summaries using the trained model (summary_model.pkl).
   * Additional experimental approaches are explored in DL_summarizer.ipynb.
4. **Output**: A concise Bengali summary.

## Limitations

* Designed exclusively for Bengali text; other languages may yield poor results.
* Summary quality depends on the training data and model performance.
* A key limitation of this model is its extractive summarization approach. It constructs summaries solely by selecting and concatenating sentences present in the original text, without performing any abstractive generation of novel content.


