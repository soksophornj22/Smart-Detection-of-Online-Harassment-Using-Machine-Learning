Report Submission: Cyberbullying Classification Project
Objective
To develop a machine learning model capable of classifying tweets into different types of cyberbullying, using natural language processing (NLP) and supervised learning techniques.

Dataset Overview
The project utilized the publicly available dataset "cyberbullying_tweets.csv" from Kaggle. This dataset contains tweets labeled with various cyberbullying categories such as age, ethnicity, gender, religion, other_cyberbullying, and not_cyberbullying. Each record includes the tweet_text and the corresponding cyberbullying_type.

After cleaning and removing rows with missing values, the dataset was preprocessed to ensure it was suitable for machine learning tasks. The final cleaned dataset consisted of several thousand labeled tweet samples, enabling both model training and evaluation.

Model Selection
This was a multi-class classification problem, aiming to categorize tweets into one of several bullying types. A combination of TF-IDF vectorization for text feature extraction and Logistic Regression for classification was selected due to its effectiveness, scalability, and interpretability in text classification problems.

Methodology
The methodology followed these core steps:

Data Preprocessing:

Removed null values.

Converted text into numerical form using TfidfVectorizer with stopword removal and a 5000-feature limit.

Target labels were kept as original class names.

Data Splitting:

The dataset was split into 80% for training and 20% for testing using train_test_split with a fixed random state for reproducibility.

Model Training & Evaluation:

Logistic Regression was trained on TF-IDF-transformed features.

Evaluation was performed using:

Confusion Matrix

Classification Report (Precision, Recall, F1-Score for each class)

Model Saving & Inference:

The trained model and vectorizer were saved using joblib.

Inference was demonstrated on new, unseen tweet examples.

Model Performance & Summary
The Logistic Regression model achieved reasonable classification performance across the different cyberbullying categories. Here are highlights of the evaluation:

Accuracy: Good overall classification accuracy, with the model able to distinguish between bullying types and non-bullying content.

F1-Score: Balanced precision and recall values across most categories, although minority classes (less frequent types of bullying) showed slightly lower performance—likely due to class imbalance.

Generalization: The model generalized well on the test set, and was able to infer the correct category of new tweets in inference tests.

Conclusion
The developed model demonstrates that text-based classification of cyberbullying is achievable with TF-IDF and Logistic Regression. For further improvement, techniques such as oversampling minority classes, using deep learning (e.g., BERT or LSTM), or incorporating sentiment and linguistic features could be explored.

The trained model is lightweight, interpretable, and deployable, making it a practical solution for initial detection of online bullying in social media platforms.
