## red-wine-quality-analysis


## Wine Quality Classification with Random Forest

This project classifies red wine quality using a Random Forest Classifier. The dataset includes various chemical properties of wine, and the goal is to predict whether a wine is of high quality (rating 7 or above).

### Project Overview

1. **Data Exploration:**
   - **Dataset:** Loaded the red wine quality dataset and explored its first few entries.
   - **Missing Values:** Verified that there are no missing values.
   - **Summary Statistics:** Analyzed statistical properties of the dataset.
   - **Visualizations:**
     - **Distribution of Wine Quality:** Shows the count of each quality rating.
       
       
![wine quality](https://github.com/user-attachments/assets/9abdb9d7-9794-429f-a004-c500ef70fd6d)



   - **Volatile Acidity vs. Wine Quality:** Visualizes how volatile acidity relates to wine quality.
       

![volatile acidity](https://github.com/user-attachments/assets/ad88d9f6-9c6a-44dc-8a97-7e8d9b69ee44)

  
       
   - **Citric Acid vs. Wine Quality:** Shows the relationship between citric acid and wine quality.
       

![citric acid vs wine quality](https://github.com/user-attachments/assets/4f89fad1-2ca4-4b07-892b-e606b280e4c8)

       
   - **Correlation Heatmap:** Displays the correlation between different features.
     

       ![correlation heatmao](https://github.com/user-attachments/assets/a77c66b4-d872-4d00-a925-6d344d87b91e)


2. **Feature Analysis:**
   - Generated a correlation heatmap to identify feature relationships.

3. **Data Preparation:**
   - Split the dataset into features and the target variable (high quality vs. not high quality).
   - Separated the data into training (80%) and testing (20%) sets.

4. **Model Training and Evaluation:**
   - **Random Forest Classifier:** Trained a Random Forest model.
   - **Performance Metrics:**
     - **Accuracy:** 93.44% on the test data.
     - **Cross-Validation Scores:** Mean CV score of 86.68%.
     - **Classification Report:** Precision, recall, and F1-score for both classes.
       - Precision: 0.95, Recall: 0.98 for class 0; Precision: 0.79, Recall: 0.59 for class 1.
     - **Confusion Matrix:** Visualized the model's prediction performance.
       

![confusion matrix](https://github.com/user-attachments/assets/d053b602-ffb6-4da8-b7e8-aa47573afe7b)



5. **Hyperparameter Tuning:**
   - **GridSearchCV:** Tuned hyperparameters for the Random Forest model.
   - **Best Parameters:**
     - `max_depth`: 10
     - `min_samples_leaf`: 1
     - `min_samples_split`: 2
     - `n_estimators`: 100
   - **Best Model Accuracy:** 93.75% on the test data.

### Key Findings

- **High Accuracy:** Achieved a high accuracy score on the test data.
- **Improved Performance:** Enhanced model performance through hyperparameter tuning.
- **Visual Insights:** Provided insights into model performance and feature relationships through various visualizations.

### Dependencies

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
