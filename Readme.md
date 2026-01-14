# Sentiment Analysis on Amazon Reviews

This project performs sentiment analysis on the **Amazon Polarity dataset** using
traditional Machine Learning, Deep Learning, and Transformer-based models.
The goal is to compare model performance and demonstrate the effectiveness of
transfer learning using BERT.

---

##  Dataset
- **Amazon Polarity Dataset** (HuggingFace)
- Binary sentiment classification:
  - 0 → Negative
  - 1 → Positive
- Review *title* and *content* are merged into a single text field

---

##  Preprocessing Steps
- Text cleaning
- Tokenization
- Label encoding
- Train / Validation / Test split
- Padding and truncation for deep learning models

---

##  Models Implemented

### 1 Logistic Regression (Baseline)
- TF-IDF feature extraction
- Used as a benchmark model

### 2 GRU (Deep Learning Model)
- Embedding layer
- GRU layer
- Dense output layer
- Early stopping applied

### BERT (Advanced Enhancement)
- Pre-trained **bert-base-uncased**
- Fine-tuned for sentiment classification
- Transfer learning approach

---

##  Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

---

##  Experimental Results

| Model | Accuracy | Precision | Recall | F1-score |
|------|----------|-----------|--------|----------|
| Logistic Regression | 0.50 | 0.91 | 0.91 | 0.91 |
| GRU | 0.49 | 0.95 | 0.96 | 0.95 |
| BERT | 0.95 | 0.95 | 0.96 | 0.95 |

BERT significantly outperforms traditional and recurrent models due to its
contextual understanding and transfer learning capability.

---

##  Model Saving
- Trained GRU and BERT models are saved to avoid retraining
- Models can be loaded later for inference or evaluation

---

## Author
## Manal Asghar
