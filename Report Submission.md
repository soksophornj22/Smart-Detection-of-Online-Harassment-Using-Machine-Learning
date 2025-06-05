# 📝 Report Submission: Cyberbullying Classification Project

## 🎯 Objective
To develop a machine learning model capable of classifying tweets based on the type of cyberbullying, leveraging natural language processing and supervised learning techniques.

## 📊 Dataset Overview
The project utilized the [Cyberbullying Classification Dataset](https://www.kaggle.com/datasets/andrewmvd/cyberbullying-classification) from Kaggle. The dataset contains labeled tweets across various categories of cyberbullying, such as:
- Age-based
- Ethnicity-based
- Gender-based
- Religion-based
- Others

The dataset was cleaned to handle missing values and standardized using **TF-IDF vectorization** to convert text data into numerical features suitable for machine learning.

## 🧠 Model Selection
This is a **multi-class classification** problem. A simple yet effective model using **TF-IDF + Logistic Regression** was implemented.

**Why Logistic Regression?**
- Easy to interpret
- Fast training time
- Solid baseline for text classification

## 🔧 Methodology
1. **Data Cleaning**  
   - Dropped rows with missing values  
2. **Text Vectorization**  
   - Used `TfidfVectorizer` from `sklearn`  
3. **Train-Test Split**  
   - 80% for training, 20% for testing  
4. **Model Training**  
   - Logistic Regression (`sklearn.linear_model`)  
5. **Evaluation**  
   - Confusion matrix  
   - Classification report (Precision, Recall, F1-score)

## ✅ Model Performance & Summary
- The model showed **strong performance** in distinguishing between different types of cyberbullying.
- **TF-IDF** helped in extracting meaningful text features.
- Evaluation metrics showed good precision and recall across classes.

### 🔮 Future Improvements
- Advanced NLP preprocessing (e.g., lemmatization, NER)
- Experimenting with ensemble models like **Random Forest** or **XGBoost**
- Fine-tuning transformer-based models like **BERT** for higher accuracy

---

📁 *This project demonstrates how basic NLP techniques and supervised learning can be combined to tackle real-world problems like cyberbullying detection.*

