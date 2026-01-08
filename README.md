# ML-PROJECT-CREDIT-CARD-FRAUD-DETECTION-

1. Introduction:  

This project implements an end-to-end Machine Learning based Credit Card Fraud Detection System. The system can learn from historical transaction data and predict whether a new transaction is fraud or legal. The project also includes handling of class imbalance, proper evaluation, and an automatic testing mechanism for easy demonstration.  

2. Problem Statement  

Credit card fraud is a serious real-world problem where illegal transactions cause financial loss to customers and banks. Fraudulent transactions are very rare compared to normal ones, which makes detection difficult. 

3. Dataset Characteristics: 

Total transactions: 284,807 

Fraudulent transactions: 492 

Legal transactions: 284,315 

Target column: Class 

0 = Legitimate Transaction 

1 = Fraudulent Transaction 

4. Features: 

Time: Time elapsed between transactions 

V1 – V28: Anonymized numerical features (PCA transformed) 

Amount: Transaction amount 

5. System Architecture and Pipeline 

This architecture ensures that the system is scalable, accurate, and suitable for real-world fraud detection scenarios. The overall system follows the pipeline shown below: 

Raw Transaction Data 

       ↓ 
       
Data Preprocessing & Scaling 

       ↓ 

SMOTE (Class Imbalance Handling) 

       ↓ 

Random Forest Model Training 
      
       ↓ 

Model Evaluation 

       ↓ 

Automatic Transaction Testing 

6. Model Design 

- Random Forest Classifier 

A Random Forest Classifier is used as the main prediction model. 

- Reasons for choosing Random Forest: 

1. Works well with tabular data 

2. Handles non-linear relationships 

3. Reduces overfitting using ensemble learning 

4. Provides high accuracy and robustness
 

7. Challenges and Limitations
   

- Challenges: 

1. Extremely imbalanced dataset 

2. Risk of overfitting after oversampling 

3. Fraud patterns may evolve over time 

- Limitations: 

1. Model trained on historical data only 

2. Real-world deployment would require continuous retraining 

3. Dataset features are anonymized, limiting interpretability 

8. Conclusion  

This project successfully demonstrates an end-to-end Credit Card Fraud Detection System using Machine Learning. By handling class imbalance with SMOTE and using a Random Forest classifier, the system achieves high performance in detecting fraudulent transactions. The inclusion of an automatic testing interface and confusion matrix visualization makes the project practical, professional, and suitable for real-world applications. 
