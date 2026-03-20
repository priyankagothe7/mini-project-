# 📰 Fake News Detection using BERT

A high-performance NLP system built to classify news articles as **Real** or **Fake** using the **Transformer** architecture. This project involves fine-tuning a pre-trained BERT model to achieve human-level accuracy in misinformation detection.

---

## 🚀 Project Overview
This project was developed as part of a 10-day intensive mini-project focused on Modern NLP. It covers the entire lifecycle of an AI project: from dataset cleaning and class imbalance handling to fine-tuning and basic deployment.

### 🧠 Model Architecture
- **Base Model:** `distilbert-base-uncased` (A lighter, faster version of BERT).
- **Library:** HuggingFace Transformers.
- **Mechanism:** Self-Attention layers used to capture long-range dependencies in news text.

---

## 📊 Performance Metrics
After fine-tuning for 3 epochs, the model achieved the following results:

| Metric    | Score |
|-----------|-------|
| Accuracy  | 98%   |
| Precision | 0.97  |
| Recall    | 0.98  |
| F1-Score  | 0.98  |

---

## 🛠️ Implementation Steps
1. **Data Preprocessing**: Merged `True.csv` and `Fake.csv`, handled missing values, and balanced class distributions.
2. **Tokenization**: Utilized the DistilBERT Tokenizer with padding and a max sequence length of 512 tokens.
3. **Fine-Tuning**: Trained using the HuggingFace `Trainer` API with an AdamW optimizer and weight decay.
4. **Evaluation**: Generated a detailed Classification Report and Confusion Matrix to identify error patterns.
5. **Deployment**: Created an interactive web UI using **Gradio** for real-time predictions.

---

## 💡 Key Learnings & Improvements
- **Class Imbalance**: Analyzed how skewed data affects precision-recall trade-offs.
- **Model Efficiency**: Comparing BERT vs. DistilBERT showed a 40% reduction in training time with minimal accuracy loss.
- **Logic over Code**: Focused on understanding *why* specific attention heads focus on sensationalist language common in fake news.

---

## 🖥️ How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/your-username/Fake-News-Detection-BERT.git](https://github.com/your-username/Fake-News-Detection-BERT.git)
