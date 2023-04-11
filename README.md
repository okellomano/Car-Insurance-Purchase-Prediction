## Car-Insurance-Purchase-Prediction
The Car Insurance Purchase Prediction project aims to build a robust machine learning model to predict the probability of customers purchasing a car insurance product.
Insurance Claim Prediction
This project aims to predict whether a customer will file an insurance claim in the next year or not, based on several features provided in the dataset. The goal is to build a binary classification model that can accurately predict whether a customer will file a claim or not.

### Dataset
The dataset used for this project contains information on insurance customers and whether they filed a claim in the last year or not. The data contains the following features:

<ul>
  <li>id: unique identifier for each customer</li>
  <li>age: age of the customer</li>
  <li>gender: gender of the customer</li>
  <li>tenure: length of time the customer has been with the insurance company</li>
  <li>region: region where the customer is located</li>
  <li>dl: whether or not the customer has a driver's license</li>
  <li>has_v_insurance: whether or not the customer has vehicle insurance</li>
  <li>v_age: age of the customer's vehicle</li>
  <li>v_accident: whether or not the customer has been in a vehicle accident in the last year</li>
  <li>v_prem_quote: the customer's vehicle insurance premium quote</li>
  <li>cs_rep: the customer's satisfaction score with the insurance company</li>
</ul>

The target variable is claim_ind, which is a binary variable indicating whether the customer filed an insurance claim in the last year or not.

### Preprocessing
The dataset was preprocessed using several steps to prepare it for modeling. These included:
<ul>
  <li>Handling missing values: missing values in the v_age and cs_rep columns were imputed using the median value of each column.</li>
  <li>Encoding categorical variables: the categorical variables gender and region were one-hot encoded to be used in the model.</li>
  <li>Scaling numerical variables: the numerical variables were scaled using a standard scaler to ensure that they were on the same scale.</li>
</ul>

### Modeling
Several machine learning models were used to predict insurance claims, including logistic regression, K-Nearest Neighbors, and Random Forest. After tuning the hyperparameters of each model, the Random Forest model performed the best with an F1 score of 0.14 and a ROC AUC of 0.74.

### Predictions
Once the model was trained, it was used to make predictions on a new dataset of insurance customers. The predicted probabilities for each customer were added to the dataset, along with a binary classification column indicating whether the customer was predicted to file a claim or not.

### Conclusion
Overall, the Random Forest model showed the best performance in predicting insurance claims. However, there is still room for improvement in the model's performance, and additional data or features could potentially improve the accuracy of the predictions.
