# Bank Marketing Data Set

This repository provides a dataset for bank marketing, which involves direct marketing campaigns conducted by a Portuguese banking institution. The campaigns were primarily based on phone calls, and the goal was to determine whether the clients would subscribe to a bank term deposit or not. The dataset contains 41,188 examples and 20 input variables.

## Dataset Description

The dataset, named "bank-additional-full.csv," consists of the following input variables:

1. Bank client data:
   - `age`: Numeric variable representing the age of the client.
   - `job`: Categorical variable indicating the type of job (e.g., 'admin.', 'blue-collar', 'entrepreneur', 'housemaid', 'management', 'retired', 'self-employed', 'services', 'student', 'technician', 'unemployed', 'unknown').
   - `marital`: Categorical variable representing the marital status (e.g., 'divorced', 'married', 'single', 'unknown').
   - `education`: Categorical variable indicating the level of education (e.g., 'basic.4y', 'basic.6y', 'basic.9y', 'high.school', 'illiterate', 'professional.course', 'university.degree', 'unknown').
   - `default`: Categorical variable specifying whether the client has credit in default (values: 'no', 'yes', 'unknown').
   - `housing`: Categorical variable indicating whether the client has a housing loan (values: 'no', 'yes', 'unknown').
   - `loan`: Categorical variable representing whether the client has a personal loan (values: 'no', 'yes', 'unknown').

2. Variables related to the last contact of the current campaign:
   - `contact`: Categorical variable denoting the contact communication type (values: 'cellular', 'telephone').
   - `month`: Categorical variable indicating the last contact month of the year (values: 'jan', 'feb', 'mar', ..., 'nov', 'dec').
   - `day_of_week`: Categorical variable representing the last contact day of the week (values: 'mon', 'tue', 'wed', 'thu', 'fri').
   - `duration`: Numeric variable indicating the last contact duration in seconds. Note that this attribute strongly affects the output target. It is advised to discard this attribute for a realistic predictive model as it is only known after the end of a call.

3. Other attributes:
   - `campaign`: Numeric variable representing the number of contacts performed during this campaign for the client.
   - `pdays`: Numeric variable indicating the number of days that passed after the client was last contacted from a previous campaign (value of 999 means the client was not previously contacted).
   - `previous`: Numeric variable representing the number of contacts performed before this campaign for the client.
   - `poutcome`: Categorical variable indicating the outcome of the previous marketing campaign (values: 'failure', 'nonexistent', 'success').

4. Social and economic context attributes:
   - `emp.var.rate`: Numeric variable representing the employment variation rate as a quarterly indicator.
   - `cons.price.idx`: Numeric variable denoting the consumer price index as a monthly indicator.
   - `cons.conf.idx`: Numeric variable indicating the consumer confidence index as a monthly indicator.
   - `euribor3m`: Numeric variable representing the Euribor 3-month rate as a daily indicator.
   - `nr.employed`: Numeric variable indicating the number of employees as a quarterly indicator.

The output variable (desired target) is:
- `y`: Binary variable representing whether the client has subscribed to a term deposit (values: 'yes', 'no') stored in the 'subscribed' column.

## Dataset Source

The dataset can be accessed from the link [here](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)

## Clustering Evaluation

To evaluate the classification performance of a K-means and a Fuzzy C-means clustering algorithm on the Bank Marketing dataset, follow these steps:

1. Download the Bank Marketing dataset from the provided link.
2. Preprocess the dataset as necessary, such as handling missing values, encoding categorical variables, and normalizing the attribute values.
3. Implement the K-means and Fuzzy C-means clustering algorithms using appropriate libraries or tools (such as scikit-learn or specialized clustering libraries).
4. Perform 5-fold cross-validation to evaluate the clustering performance.
5. Calculate the confusion matrix, sensitivity, specificity, total accuracy, F1-score, ROC curve, and area under the curve (AUC) for each clustering algorithm.
6. Analyze the results to gain insights into the clustering algorithms' performance.

## Acknowledgments

The Bank Marketing Data Set was sourced from the UCI Machine Learning Repository.
