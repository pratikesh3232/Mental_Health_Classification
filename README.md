# Mental Health Prediction

This project aims to predict the likelihood of depression based on various individual factors such as age, profession, lifestyle, and mental health history. The model is trained on a dataset from the Kaggle Playground Series Season 4, Episode 11 competition ([link][(https://www.kaggle.com/competitions/playground-series-s4e11/overview)]). 

**Approach:**

The project involves the following key steps:

1. **Data Cleaning and Preprocessing:**
   - Handling missing values by imputation and strategic replacements based on logical relationships between features.
   - Standardizing column names for consistency.
   - Removing categories with low frequency to reduce noise.
   - Consolidating similar categories in features like 'sleep_duration' and 'dietary_habits'.
   - Converting categorical variables into numerical representations using label encoding.

2. **Feature Engineering and Scaling:**
    - Scaling numerical features using StandardScaler to improve model performance.

3. **Model Training and Selection:**
   - Exploring various machine learning algorithms:
     - Logistic Regression 
     - Decision Tree
     - Random Forest 
     - Support Vector Machine 
     - k-nearest neighbor
     - Gradient Boosting 
     - AdaBoost 
     - LGBM 
   - Evaluating model performance using accuracy and classification report metrics.
   - Implementing a Voting Classifier to combine predictions from multiple models for improved robustness and accuracy.

4. **Prediction and Submission:**
   - Applying the trained Voting Classifier to the test dataset to predict depression likelihood.
   - Generating a submission file in the required format for the Kaggle competition.

**The Voting Classifier, combining the predictions of 8 different models, achieved an accuracy of over 0.93891 on the validation set.** This demonstrates the effectiveness of the chosen approach in predicting depression based on the given features.

