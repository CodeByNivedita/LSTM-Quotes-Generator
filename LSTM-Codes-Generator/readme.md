# LSTM Quotes Generator

This project implements a deep learning–based **LSTM text generation model** trained on a curated dataset of English quotes.  
The goal is to generate new, coherent, quote-style sentences by learning patterns from thousands of cleaned and preprocessed quotes.

---

##  Project Overview->

This project demonstrates:

1- Deep Learning pipeline for NLP text generation  
2- Data cleaning & preprocessing for large text datasets  
3- Tokenization and sequence modeling  
4- Building and training an LSTM-based language model  
5- Generating new quotes from a seed text  

The project is ideal for learning sequence modeling concepts and showcasing practical NLP experience in a portfolio or resume.

---

## 📂 Dataset

The dataset is taken originally from Kaggle.
Link for dataset->"https://www.kaggle.com/datasets/sanjeetsinghnaik/quotes-from-goodread"
The dataset originally contained **30,000+ quotes** with multiple issues:

- Missing authors  
- Mixed languages  
- Duplicate quotes  
- Special characters  
- Inconsistent formatting  

A preprocessing pipeline was applied to:

- Remove non-English quotes  
- Clean and normalize text  
- Correct author names  
- Remove duplicates  
- Drop irrelevant or broken rows  

The final dataset contains **~2,800 clean English quotes** ready for modeling.

---

## 🧹 Data Preprocessing Steps

1. Removed special characters and non-ASCII symbols  
2. Filtered out non-English quotes using `langid`  
3. Cleaned author names (removed starting dashes, book titles, etc.)  
4. Removed rows with missing or invalid authors  
5. Dropped duplicates based on the quote text  
6. Stripped extra whitespace and normalized text  
7. Sampled manageable dataset for efficient training  

---

## 🔧 Model Architecture

A simple yet effective LSTM structure:
Embedding Layer (word embeddings)
LSTM Layer (128 units)
Dense Layer (ReLU)
Output Dense Layer (Softmax)
