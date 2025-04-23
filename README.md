# 🎬 Movie Trailer Sentiment Analysis with PyTorch & HuggingFace

Predict whether a **movie trailer** will be a **Hit, Flop, or Average** based on real-time YouTube comments. This deep learning + NLP-powered project combines state-of-the-art transformer models with traditional sentiment analysis tools to classify public opinion on upcoming films.

---

## 📌 Table of Contents

- [🔍 Overview](#-overview)
- [🚀 Tech Stack](#-tech-stack)
- [📁 Project Structure](#-project-structure)
- [⚙️ How It Works](#️-how-it-works)
- [💡 Features](#-features)
- [🧪 Sample Output](#-sample-output)
- [🛠️ Installation & Usage](#️-installation--usage)
- [📈 Future Enhancements](#-future-enhancements)
- [🙋 Author](#-author)

---

## 🔍 Overview

This project scrapes YouTube comments from any movie trailer using the **YouTube Data API**, performs **sentiment analysis** using both rule-based and transformer-based models, and classifies the overall audience reaction as:

- 🎯 **Hit**
- ⚠️ **Average**
- ❌ **Flop**

---

## 🚀 Tech Stack

| Tool/Library      | Role                              |
|-------------------|------------------------------------|
| `PyTorch`         | Deep learning backend              |
| `HuggingFace Transformers` | BERT-like sentiment classification |
| `NLTK`            | Preprocessing, tokenization       |
| `VADER`           | Rule-based sentiment scoring      |
| `YouTube API`     | Fetch YouTube comments            |
| `Pandas` / `Matplotlib` | Data analysis and visualization |

---

## 📁 Project Structure

youtube-sentiment-analysis/ ├── sentiment_model.ipynb # Transformer + VADER-based classifier ├── youtube_comments_fetcher.txt # Pulls comments via YouTube Data API ├── datasets/ │ └── trailer_comments.xlsx # Sample Excel dataset ├── README.md # This file

---

## ⚙️ How It Works

1. 🔗 **Enter YouTube Trailer URL**
2. 📥 Fetch top comments via **YouTube API**
3. 🧹 Preprocess (remove emojis, stopwords, non-text content)
4. 🧠 Classify each comment using:
   - ✅ **HuggingFace Transformer Model**
   - ✅ **VADER Sentiment Intensity Analyzer**
5. 📊 Aggregate results:
   - >60% positive ➝ **Hit**
   - ~40–60% neutral/mixed ➝ **Average**
   - <40% positive ➝ **Flop**
6. ✅ Output the verdict with sentiment stats

---

## 💡 Features

- 🎥 Supports **any YouTube movie trailer**
- 🤖 Combines **deep learning + rule-based** NLP
- 🇮🇳 Handles **Indian language** comments
- 📊 Visualization of sentiment spread (optional)
- 🧪 Works offline with sample datasets too

---

📈 Future Enhancements
🌐 Deploy as a Flask or Streamlit web app

🔍 Improve multilingual support with IndicBERT or XLM-R

🧠 Fine-tune sentiment models on regional datasets

---

🙋 Author
Nikhil Nemala
📧 nemalanikhil7@gmail.com
🌐 GitHub: @Nikhilnemala
🔗 LinkedIn: [linkedin.com/in/your-profile](https://www.linkedin.com/in/nikhil-nemala-643443275/)