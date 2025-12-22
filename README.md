# ML File Sorter

A smart Python tool to organize and sort text documents into directory structures based on their content using Zero-Shot Classification.

This project provides a command-line tool to scan a directory of unsorted files, analyze their text content to determine their category (e.g., "Finance," "Personal," "Work"), and move them into appropriate sub-folders.

---

## Repository Structure

```
ml-file-sorter/
├── input_data/
│   ├── document_1.txt
│   └── document_2.txt
├── sorted_output/
├── main.py
├── classifier.py
├── README.md
└── .gitignore
```

---

## Machine Learning Components

This tool uses:

- **Zero-Shot Classification**: A machine learning technique that allows the model to classify text into categories it hasn't explicitly been trained on.
  Example: You provide the labels ["Invoice", "Resume", "Recipe"], and the model determines which label best fits the text, even if it has never seen your specific invoices before.

- **Hugging Face Transformers**: A library for state-of-the-art Natural Language Processing (NLP).

- **Pre-trained Model (facebook/bart-large-mnli)**: This project utilizes a pre-trained model optimized for Natural Language Inference (NLI). The script loads this model to compare the document text against your defined folder names to predict the correct category with high confidence.

---

## Setup
(Pending build)

---

## Usage
(Pending build)
