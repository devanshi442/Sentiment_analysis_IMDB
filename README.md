# 🎬 Sentiment Analysis using DistilBERT (IMDB Dataset)

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

A deep learning NLP project that classifies movie reviews as **positive** or **negative** using the powerful DistilBERT transformer model, fine-tuned on the IMDB dataset.

---

## 📌 Overview

This project demonstrates an end-to-end sentiment classification pipeline using modern NLP techniques. It fine-tunes a pre-trained `distilbert-base-uncased` model to achieve high accuracy on binary sentiment classification, showcasing the effectiveness of transformer-based architectures over traditional ML approaches.

---

## 🧠 Tech Stack

| Tool | Purpose |
|------|---------|
| Python 🐍 | Core language |
| Hugging Face Transformers 🤗 | Pre-trained DistilBERT model |
| Hugging Face Datasets | IMDB data loading |
| PyTorch 🔥 | Model training & inference |
| Scikit-learn | Evaluation metrics |
| NLTK | Text preprocessing |

---

## ⚙️ Features

- ✅ Text preprocessing using NLTK (stopword removal, tokenization, HTML cleaning)
- ✅ Transformer-based model (`distilbert-base-uncased`) with classification head
- ✅ Fine-tuning on IMDB with AdamW optimizer and learning rate scheduler
- ✅ Evaluation using: **Accuracy**, **Precision**, **Recall**, **F1-score**
- ✅ Clean, reproducible notebook-based pipeline

---

## 📂 Dataset

**IMDB Movie Reviews Dataset**
- 50,000 reviews (25k train / 25k test)
- Binary classification:
  - 😊 Positive
  - 😞 Negative

Loaded directly via the Hugging Face `datasets` library:
```python
from datasets import load_dataset
dataset = load_dataset("imdb")
```

---

## 🏗️ Project Workflow

1. **Data Loading** — Load IMDB dataset using Hugging Face `datasets`
2. **Preprocessing** — Remove HTML tags, filter stopwords, tokenize with DistilBERT tokenizer
3. **Model Setup** — Load `distilbert-base-uncased` with a binary classification head
4. **Fine-tuning** — Train using AdamW optimizer with a linear learning rate scheduler
5. **Evaluation** — Report classification metrics using `sklearn.metrics`

---

## 📊 Results

The fine-tuned DistilBERT model demonstrates strong performance on the IMDB test set, significantly outperforming traditional ML baselines (TF-IDF + Logistic Regression, etc.).

> Detailed metrics (accuracy, F1, confusion matrix) are available in the notebook output.

---

## ▶️ How to Run

### Option 1: Google Colab (recommended)

1. Open the notebook in [Google Colab](https://colab.research.google.com)
2. Install dependencies:
```bash
pip install transformers datasets scikit-learn nltk torch
```
3. Run all cells sequentially

### Option 2: Local Setup
```bash
# Clone the repository
git clone https://github.com/your-username/sentiment-analysis-distilbert.git
cd sentiment-analysis-distilbert

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook
```

---

## 📸 Sample Output
```
Review: "This movie was absolutely fantastic! A masterpiece."
Sentiment: POSITIVE ✅ (confidence: 98.3%)

Review: "Terrible plot, awful acting. Complete waste of time."
Sentiment: NEGATIVE ❌ (confidence: 96.7%)
```

---

## 🔮 Future Improvements

- [ ] Deploy as a web app using Streamlit or Flask
- [ ] Add real-time sentiment prediction via REST API
- [ ] Experiment with BERT, RoBERTa, and ALBERT
- [ ] Support multi-class sentiment (neutral, mixed)
- [ ] Add explainability with attention visualization

---

## 🙋‍♀️ Author

**Devanshi Saxena**


---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---
