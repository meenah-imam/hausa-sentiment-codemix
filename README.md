# hausa-sentiment-codemix
# Hausa Sentiment Analysis: Code-Mix vs Monolingual

This project investigates the performance of sentiment analysis models on **Hausa language data**, comparing:

* Monolingual Hausa text
* Code-mixed Hausa-English text
* Combined datasets

The goal is to understand how **code-mixing affects model performance** in low-resource African NLP.

---

## Dataset

The experiment uses the **AfriSenti Hausa dataset** (Muhammad et al., 2023), accessed via Hugging Face.

* ~22,000 tweets
* Pre-split into train, validation, and test
* Labels: Positive, Negative, Neutral

---

## Methodology

The study follows a controlled experimental setup:

1. Load and preprocess Hausa tweets
2. Create:

   * Monolingual dataset
   * Code-mixed dataset
   * Combined dataset
3. Train transformer-based models (e.g., XLM-RoBERTa)
4. Evaluate performance using:

   * Accuracy
   * F1-score
   * Confusion matrix

---

## Experiments

Three training conditions:

* **Monolingual only**
* **Code-mixed only**
* **Combined dataset**

All datasets are **size-matched** to ensure fair comparison.

---

## Results

Results include:

* Class distribution analysis
* Model performance metrics
* Visualizations of comparison across setups

(See `/outputs/figures` for plots)

---

##  How to Run

### 1. Install dependencies

```bash
pip install -r requirements.txt
```

### 2. Run notebook

```bash
jupyter notebook notebooks/Codemix_vs_Monolingual.ipynb
```

---

##  Requirements

* Python 3.10+
* PyTorch
* Hugging Face Transformers
* Datasets
* Scikit-learn
* Matplotlib

---

##  Citation

If you use this work, please cite:

AfriSenti:
Muhammad et al. (2023)

---

##  Author

Amina Imam Abubakar
PhD in Applied AI (NLP)
Focus: Low-resource African languages, Sentiment Analysis

---

##  Notes

This project is part of ongoing research on:

* Code-mixing in African NLP
* Low-resource language modeling
* Responsible AI in multilingual systems
