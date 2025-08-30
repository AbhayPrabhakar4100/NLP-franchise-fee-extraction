# nlp-franchise-fee-extraction

## 📌 Project Overview
This project leverages **Natural Language Processing (NLP)** to extract structured financial details from **franchise disclosure documents**, with a focus on **Item 5: Initial Fees**.  
The aim is to reduce manual effort in analyzing franchise agreements by applying **frequency-based text analysis, topic modeling, and transformer-based Question Answering (Q&A)**.

---

## 📦 Dataset
- **Documents:** 50 U.S. franchise disclosure files  
- **Target Section:** "Item 5: Initial Fees"  
- **Content Extracted:** Key financial terms, fee structures, and direct answers to fee-related queries  

---

## 🔬 Methodology
### 1. Frequency & Term Analysis
- **Bag of Words (BoW):** Identified recurring legal/financial terms  
- **N-Gram Analysis:** Extracted common bigrams for added context  
- **TF-IDF:** Highlighted unique, document-specific words  

### 2. Topic Modeling
- **K-Means Clustering:** Grouped franchises (e.g., food vs. non-food businesses)  
- **Sentence-BERT Embeddings:** Captured semantic similarity to discover hidden topics  

### 3. Question Answering (Q&A)
- **Model:** RoBERTa (pre-trained transformer)  
- **Objective:** Automatically extract the **initial franchise fee**  
- **Sample Queries:**  
  - “What is the initial fee?”  
  - “What is the initial franchise fee in dollars?”  
  - “What is the standard nonrefundable franchise fee?”  

---

## ✅ Key Results
- **Best-performing query:** *“What is the initial franchise fee in dollars?”*  
- **F1-score:** 0.76 using RoBERTa Q&A model  
- **Clustering insights:** Clear separation of franchise types by business model and fee structure  

---

## 📂 Repository Contents
- `chik-fil-a.ipynb` → NLP pipeline applied to Chick-fil-A disclosure data  
- `Combination_of_Methods_Item5.ipynb` → Integrates frequency-based + embedding methods  
- `QnA_BERT_VS_v1_1.ipynb`, `QnA_BERT_VS_v2.ipynb` → RoBERTa-based Q&A experiments  
- `Word_Cloud_Visualization.ipynb` → Word cloud generation of key financial/legal terms  
- `FourQuestions_m.csv`, `FourQuestions_roberta_m.csv` → Extracted Q&A results  
- `Report_Extracting_Info_NLP.pdf` → Full project report  

---


