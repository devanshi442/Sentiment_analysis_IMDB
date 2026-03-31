🎬 Sentiment Analysis using DistilBERT (IMDB Dataset)

🚀 A deep learning NLP project that classifies movie reviews as positive or negative using the powerful DistilBERT transformer model.

📌 Overview

This project demonstrates an end-to-end sentiment classification pipeline using modern NLP techniques. It leverages a pre-trained transformer model to achieve high accuracy on the IMDB dataset.

🧠 Tech Stack
Python 🐍
Hugging Face Transformers 🤗
DistilBERT
Scikit-learn
NLTK
PyTorch
⚙️ Features
✔️ Text preprocessing using NLTK (stopwords, tokenization)
✔️ Transformer-based model (DistilBERT)
✔️ Efficient training & inference
✔️ Evaluation using:
Accuracy
Precision
Recall
F1-score
📂 Dataset
IMDB Movie Reviews Dataset
Binary classification:
Positive 😊
Negative 😞
🏗️ Project Workflow
Data loading using Hugging Face datasets
Text preprocessing (cleaning, tokenization)
Model loading using DistilBERT
Training and fine-tuning
Evaluation using sklearn metrics
📊 Results

The model demonstrates strong performance in sentiment classification, showcasing the effectiveness of transformer-based architectures over traditional ML approaches.

▶️ How to Run
Open the notebook in Google Colab

Install dependencies:

pip install transformers datasets scikit-learn nltk
Run all cells
📸 Sample Output
Predicts sentiment of movie reviews
Outputs classification metrics
🙋‍♀️ Author

Devanshi Saxena

🌟 Future Improvements
Deploy as a web app (Streamlit / Flask)
Add real-time sentiment prediction
Experiment with other transformer models (BERT, RoBERTa)
