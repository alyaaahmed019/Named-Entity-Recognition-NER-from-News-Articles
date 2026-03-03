# 🧠 Named Entity Recognition (NER) — Rule-Based vs spaCy

This project implements and evaluates different approaches for **Named Entity Recognition (NER)** using the CoNLL-2003 English dataset.

The objective is to compare a custom **rule-based NER system** with pretrained statistical models from spaCy.

---

## 📌 Project Overview

This notebook includes:

- Data loading from CoNLL format
- BIO tag extraction
- Exploratory Data Analysis (EDA)
- Rule-based NER implementation
- Model-based NER using spaCy
- BIO tag alignment and mapping
- Performance evaluation
- Visualization of results

---

## 📂 Dataset

The project uses the **CoNLL-2003 English dataset**, which contains manually annotated named entities.

Entity types:

- **PER** — Person  
- **ORG** — Organization  
- **LOC** — Location  
- **MISC** — Miscellaneous  

---

## ⚙️ Implemented Approaches

### 1️⃣ Rule-Based NER

A heuristic-based system using:

- Capitalization rules  
- Consecutive uppercase token detection  
- Organization keyword matching  
- Location dictionary matching  
- Simple person-name pattern detection  

---

### 2️⃣ Model-Based NER

Pretrained spaCy models:

- `en_core_web_sm`
- `en_core_web_lg`

Entities are mapped to BIO format to ensure consistent evaluation with the dataset labels.

---

## 📊 Evaluation Metrics

Models are evaluated using:

- Precision  
- Recall  
- F1-score  
- Macro F1-score  

The notebook provides:

- Classification reports  
- Label distribution visualization  
- Sentence length histogram  
- Model comparison bar chart  

---

## 🛠 Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- scikit-learn  
- spaCy  

---

## 🚀 How to Run

1. Install dependencies:

```bash
pip install spacy pandas numpy matplotlib scikit-learn
python -m spacy download en_core_web_sm
python -m spacy download en_core_web_lg
