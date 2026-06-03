# 📰 News Topic Classifier Using BERT

## 🎯 Objective of the Task

The objective of this project is to fine-tune a Transformer-based model (BERT) to automatically classify news headlines into topic categories. The project demonstrates the use of modern NLP techniques for text classification and provides a live interface for real-time predictions.

---

## 🛠️ Methodology / Approach

- Loaded the AG News dataset from Hugging Face Datasets.
- Preprocessed and tokenized the news headlines using the BERT tokenizer.
- Fine-tuned the pretrained `bert-base-uncased` model using the Hugging Face Transformers library.
- Trained the model for news topic classification across four categories:
  - World
  - Sports
  - Business
  - Sci/Tech
- Evaluated the model using:
  - Accuracy Score
  - Weighted F1-Score
- Saved the best-performing model checkpoint.
- Deployed the trained model using Gradio to enable live user interaction and real-time predictions.

---

## 📊 Dataset Used

**AG News Dataset** (Hugging Face)

The dataset contains news headlines categorized into four classes:

- 🌍 World
- ⚽ Sports
- 💼 Business
- 🔬 Sci/Tech

---

## 🤖 Model Applied

- BERT (`bert-base-uncased`)

---

## 🛠️ Libraries Used

- transformers
- datasets
- torch
- scikit-learn
- pandas
- numpy
- gradio

---

## 📈 Key Results or Observations

- The fine-tuned BERT model successfully classified news headlines into their respective categories.
- The model achieved **91.10% Accuracy** and **91.09% Weighted F1-Score** on the validation dataset.
- Sports headlines were classified with the highest accuracy due to their distinctive terminology.
- Some overlap was observed between Business and Sci/Tech categories because of similar vocabulary.
- The deployed Gradio application enabled users to test custom headlines and receive instant predictions with confidence scores.
---
<img width="1107" height="545" alt="image" src="https://github.com/user-attachments/assets/487cde8f-5067-4d78-95be-d33d8fe46049" />

---
**Confusion Matrix**


<img width="614" height="590" alt="image" src="https://github.com/user-attachments/assets/feaf99ae-4a4f-47a5-8395-790eecab6998" />

---

The fine-tuned model is deployed on Hugging Face Space : [news-topic-classifier-BERT](https://huggingface.co/spaces/johnasad09/news-topic-classifier-bert)
