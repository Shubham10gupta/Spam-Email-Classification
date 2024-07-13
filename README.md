# Spam-Email-Classification
Spam email classification is crucial for filtering unsolicited emails. Using the UCI SPAM E-mail Database with 4601 instances and 57 features, we build a machine learning model to distinguish spam from non-spam. Key steps include data preprocessing, exploratory analysis, model training  and evaluation, achieving robust email filtering.
### Spam Email Classification

#### Overview
Spam email classification is a critical task in natural language processing and cybersecurity, aiming to distinguish between legitimate emails and spam. Spam emails include unwanted advertisements, phishing attempts, and other unsolicited messages. The goal of this project is to build a machine learning model that can accurately classify emails as spam or not spam using the SPAM E-mail Database from the UCI Machine Learning Repository.

#### Dataset
The dataset used in this project is the SPAM E-mail Database from the UCI Machine Learning Repository. It contains 4601 instances with 57 continuous features and 1 nominal class label indicating whether an email is spam (1) or not spam (0). The features include the frequency of specific words and characters in the email and various metrics related to sequences of capital letters.

#### Data Characteristics
- **Number of Instances**: 4601
- **Number of Attributes**: 58 (57 continuous, 1 nominal class label)
- **Class Distribution**: 39.4% spam, 60.6% non-spam
- **Attributes**:
  - `word_freq_WORD`: Percentage of words in the email that match a specific word (e.g., 'word_freq_make').
  - `char_freq_CHAR`: Percentage of characters in the email that match a specific character (e.g., 'char_freq_!').
  - `capital_run_length_average`: Average length of uninterrupted sequences of capital letters.
  - `capital_run_length_longest`: Length of the longest uninterrupted sequence of capital letters.
  - `capital_run_length_total`: Total number of capital letters in the email.

#### Methodology
The project involves the following steps:

1. **Data Loading and Preprocessing**:
   - Load the dataset and assign appropriate feature names.
   - Separate features and labels.
   - Split the data into training and testing sets.
   - Standardize the features for better model performance.

2. **Exploratory Data Analysis (EDA)**:
   - Examine the dataset structure and class distribution.
   - Visualize feature correlations to identify patterns.

3. **Feature Selection**:
   - Although all features are initially used, feature selection can be performed to improve model performance and reduce overfitting.

4. **Model Training and Evaluation**:
   - Train a Logistic Regression model and evaluate its performance using accuracy, classification report, and confusion matrix.
   - Consider using other models like Decision Trees, Random Forests, and Support Vector Machines (SVM) for comparison.

5. **Hyperparameter Tuning**:
   - Use GridSearchCV to find the best hyperparameters for the Logistic Regression model.
   - Evaluate the best model on the test set and compare its performance with the initial model.

6. **Model Testing**:
   - Validate the model on unseen data to ensure its generalizability.

#### Results
The Logistic Regression model achieved significant accuracy in distinguishing between spam and non-spam emails. Hyperparameter tuning further improved the model's performance, making it a robust solution for spam email classification.

#### Conclusion
The spam email classification project demonstrates the effectiveness of machine learning in identifying spam emails. By leveraging the SPAM E-mail Database, the project showcases the steps involved in preprocessing, analyzing, and modeling data for accurate email classification. The final model can be integrated into email systems to filter out spam and enhance email security.
