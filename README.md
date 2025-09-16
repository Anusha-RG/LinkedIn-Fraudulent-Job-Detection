# LinkedIn Fraudulent Job Detection  

## 📌 Overview  
This project investigates the rising issue of **fraudulent job postings on LinkedIn** and proposes an automated detection system using **Machine Learning (ML)** and **Natural Language Processing (NLP)** techniques.  

The system analyzes job descriptions, recruiter behaviors, and contextual indicators of legitimacy to distinguish between **genuine job opportunities** and **scams**. By leveraging classification algorithms on real-world datasets, the project demonstrates how ML can improve the **safety and trustworthiness of digital job markets**.  

This repository contains:  
- Source code for the ML/NLP pipeline (`cse291d_final_project.py`)  
- Processed results and evaluations  
- Research paper: *LinkedIn Fraudulent Job Detection* (`LinkedIn_Job_Detection.pdf`)  

---

## 📊 Research Motivation  
- LinkedIn has over **930M users (2023)**, making it a prime target for fraud.  
- Job scams increased by **118% in 2023**, leading to financial and data losses.  
- Fraudulent postings mimic legitimate ones using tactics like vague job descriptions, inflated salaries, and suspicious recruiter info.  
- Our goal: build a **scalable ML framework** to automatically detect and mitigate fraudulent job ads.  

---

## 📂 Dataset  
We used two primary datasets:  

1. **Employment Scam Aegean Dataset (EMSCAD)**  
   - ~17,880 real-world job ads (2012–2014)  
   - 17,014 legitimate ads, 866 fraudulent ads  
   - Published in MDPI *Future Internet Journal*  

2. **LinkedIn Job Postings Dataset (2023–2024)**  
   - ~124,000 LinkedIn job ads with metadata (title, description, salary, location, recruiter info, etc.)  

Additionally, a **user survey** was conducted to gather real-world red flags from job seekers.  

---

## ⚙️ Methodology  
1. **Data Preprocessing**  
   - Text cleaning, tokenization, TF-IDF feature extraction  
   - Balanced dataset using sampling techniques  

2. **Model Training**  
   - Trained **Multinomial Naive Bayes** on EMSCAD  
   - Applied predictions on LinkedIn dataset to label suspicious jobs  
   - Trained **Logistic Regression** on enriched LinkedIn data  

3. **Evaluation Metrics**  
   - Confusion Matrix  
   - Precision, Recall, F1-score  

---

## 🚀 Results & Key Findings  
- Fraudulent job postings often **mirror description length** of legitimate ones.  
- Scams are concentrated in **major metros** (NYC, Chicago, Houston), but smaller cities (Phoenix, Charlotte) show **disproportionately high fraud rates**.  
- Red flags include:  
  - Overuse of “urgent,” “guaranteed,” “no experience”  
  - Suspicious **toll-free phone numbers**  
  - Targeting **customer service roles** the most (~300 scams identified)  

---

## 📌 Limitations  
- Models trained on static datasets → may not generalize well to new fraud tactics.  
- Class imbalance: fewer fraudulent samples may bias results.  
- Limited features: more advanced embeddings (BERT, contextual analysis) could improve detection.  

---

## 🔮 Future Work  
- Develop a **web app tool** for real-time scam detection.  
- Implement **continuous learning models** to adapt to evolving scam tactics.  
- Explore correlations between **economic cycles** and scam surges.  

---

## 🛠️ Installation & Usage  

### Requirements  
- Python 3.8+  
- Install dependencies and clone the repo to run:  
  ```bash
  git clone https://github.com/Anusha-RG/LinkedIn-Fraudulent-Job-Detection.git
  python cse291d_final_project.py

##👩‍💻 Authors

- Anusha Ravichandran, University of California, San Diego
- Pooja Sounder Rajan, University of California, San Diego
