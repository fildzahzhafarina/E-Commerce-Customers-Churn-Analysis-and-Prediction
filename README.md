# Final Project Data Science Rakamin Academy - Ecommerce Customer Churn Prediction
## Stage 1
EDA Data

Summary dari EDA:
- Split data train and data test (80:20)
- PreferredLoginDevice: combine category "Mobile Phone" menjadi "Phone"
- Label Encoding : Gender 
- One Hot Encoding : Category Feature
- Handle missing value
- Prevent multicolinearity
- Check Outlier ( data is reasonable and real )

## Stage 2
Do all the things listed on the Stage 1 summary

## Stage 3 
**Split Data Train & Test**: Split data train and test have been carried out at the preprocessing stage to avoid data leaks, because the test data is unseen data.
Modeling:  
- Decision Tree (best model before hyperparameter tuning)
- Xgboot
- Catboost (best model after hyperparameter tuning)
- Adaboost
- Random forest 
- Logistic Regression

**Model Evaluation**: 
In the case of Ecommerce churn prediction, we use Recall as the main metric because the main purpose of this prediction model is to prevent customers from churn if churn is detected, therefore with our prediction recall metrics we can focus on as many customers as possible to churn to prevent churn. them to churn.

## Stage 4
Customers who are predicted to churn will be checked on the complaint data. If the customer complains, the customer goes into the priority category. Meanwhile, if the customer does not complain, go to regular customer service. If the customer is predicted to churn but does not complain, an offer will be given according to the customer's shopping behavior

Even though the model that has been trained has passed the baseline model, which means the model is good enough, the model is not yet the best-fit because a better model can still be found by trying to use other features on the data that was dropped in the preprocess stage (stage 2.), and can fine-tune hyperparameters

