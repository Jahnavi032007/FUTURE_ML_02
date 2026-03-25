# 🎫 Support Ticket Classification & Prioritization — FUTURE_ML_02

## 🔍 Objective

The objective of this project is to build a Machine Learning system that can automatically:

- Classify customer support tickets into categories  
- Assign priority levels (High / Medium / Low)  

This helps businesses improve response time, reduce manual effort, and enhance customer satisfaction.

---

## 📦 Dataset

Dataset Used:  
Customer Support Ticket Dataset  

🔗 Dataset Link:  
https://www.kaggle.com/datasets/suraj520/customer-support-ticket-dataset  

The dataset contains real-world support tickets including:

- Ticket Subject (text input)
- Ticket Type (category label)
- Ticket Priority (existing priority)

Due to file size limitations, the dataset is not included in this repository.

---

## 🛠 Tools & Technologies

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- NLTK  
- TF-IDF Vectorization  
- Google Colab  

---

## 🚀 Project Workflow

### 1️⃣ Data Loading & Understanding
- Loaded dataset using Pandas  
- Identified relevant columns:  
  - Ticket Subject → input text  
  - Ticket Type → classification label  

---

### 2️⃣ Text Preprocessing
- Converted text to lowercase  
- Removed punctuation and special characters  
- Removed stopwords using NLTK  

---

### 3️⃣ Feature Engineering
- Converted text into numerical form using TF-IDF  
- Used n-grams (unigrams + bigrams) to capture patterns  

---

### 4️⃣ Model Training
- Used Logistic Regression for multi-class classification  
- Trained model on processed text features  

---

### 5️⃣ Model Evaluation

Metrics used:
- Accuracy  
- Precision  
- Recall  
- F1-score  

### 📊 Results

Accuracy: **20.24%**

The model performance is limited due to dataset characteristics such as overlapping categories and similar vocabulary across classes.

---

## ⚠ Model Performance Note

The model achieved ~20% accuracy, which is close to a random baseline due to the nature of the dataset.

### Challenges:
- High similarity between categories (e.g., Billing vs Refund)
- Short and ambiguous ticket descriptions
- Overlapping vocabulary across classes

Despite this, the project successfully demonstrates:

✔ End-to-end NLP pipeline  
✔ Text preprocessing and feature engineering  
✔ Multi-class classification  
✔ Priority assignment logic  
✔ Business use-case implementation  

### Future Improvements:
- Use larger and cleaner datasets  
- Apply advanced models (XGBoost, BERT)  
- Use domain-specific feature engineering  

---

## ⚡ Priority Assignment System

A rule-based system was implemented to assign priority:

- High → urgent, failed, error  
- Medium → delay, slow  
- Low → general queries  

This simulates real-world decision-making in support systems.

---

## 📈 Business Impact

This system helps organizations:

- Automatically categorize incoming tickets  
- Identify urgent issues quickly  
- Reduce manual sorting effort  
- Improve support response time  
- Enhance customer experience  

---

## 📁 Repository Structure

FUTURE_ML_02  
│  
├── FUTURE_ML_02_Support_Ticket_Classification.ipynb  
└── README.md  

---

## ▶ How to Run

1. Download dataset from Kaggle  
2. Upload dataset in Google Colab  
3. Run all cells sequentially  
4. Test using custom input tickets  

---

## ✅ Conclusion

This project demonstrates how Machine Learning can be applied to automate customer support operations.

Even with dataset limitations, the system showcases a complete NLP pipeline and highlights how intelligent ticket classification can improve business efficiency.
