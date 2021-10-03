# Predicting Mobile Payment Using Machine Learning Methods

This is a repository containing the Jupyter Notebooks for my data science project on predicting mobile payment adoption.

## Motivation and Background

The goal of this project is to provide insights on the **characteristics of mobile payment adopters**, defined as those who have used tap-and-pay at the point of sale in the last 12 months.

- This question is of interest to *merchants and especially small businesses*, who may consider whether to accept mobile payment in store. By comparing characteristics of target consumers and mobile payment adopters, businesses can evaluate the potential benefit and cost of accepting mobile payment.

-  *Mobile payment app developers* may also be interested in knowing the characteristics of likely adopters for marketing purposes and room for potential expansion.

I use data from the [**2019 Survey of Consumer Payment Choice**](https://www.atlantafed.org/banking-and-payments/consumer-payments/survey-of-consumer-payment-choice/2019-survey.aspx), a yearly survey conducted by the Federal Reserve Bank of Atlanta, for the project.

## High-level findings

To address the questions, I did exploratory data analysis and trained supervised machine learning models to predict mobile payment adoption. 

**Exploratory data analysis**

- EDA shows that a number of demographic factors (e.g., age, education, employment status) are positively related to mobile payment adoption. However, since features are correlated, it is hard to tell which factor may predict adoption the best.

**Supervised machine learning**

- The best performing model is XGBoost Classifier, with an F1-score of 0.411, precision of 0.315 and recall of 0.590, among logistic regression with lasso and ridge penalty and random forest.
  
  - The baseline logistic regression model (without regularization) with F1-score of 0.181.
  
- The ten most important features for prediction are: whether a person is currently working, age, education, number of hours working, education, adoption of debit and credit card, household income, and (certain) census divisions.


## Links to notebook

Please check out the following notesbooks for details of the exploratory data analysis, model training and results:


- [Exploratory Data Analysis](https://github.com/sharonshiao/predicting_mobile_payment_adoption/blob/ab82b1e05194664dffc5f0293d19b7dcb4d1e865/notebooks/Exploratory_data_analysis.ipynb)

- [Model training](https://github.com/sharonshiao/predicting_mobile_payment_adoption/blob/ab82b1e05194664dffc5f0293d19b7dcb4d1e865/notebooks/Model_training.ipynb)



## References

Federal Reserve Bank of Atlanta. (2020, May 19). 2019 SCPC Questionnaire. Retrieved September 26, 2021, from [https://www.atlantafed.org/-/media/documents/banking/consumer-payments/survey-of-consumer-payment-choice/2019/2019_SCPC_Questionnaire.pdf.](https://www.atlantafed.org/-/media/documents/banking/consumer-payments/survey-of-consumer-payment-choice/2019/2019_SCPC_Questionnaire.pdf)

Foster, K. (2020, April 10). Codebook and Data Guide to the 2019 Survey of Consumer Payment Choice. Retrieved September 26, 2021, from [https://www.atlantafed.org/-/media/documents/banking/consumer-payments/survey-of-consumer-payment-choice/2019/scpc_2019_codebook.pdf.](https://www.atlantafed.org/-/media/documents/banking/consumer-payments/survey-of-consumer-payment-choice/2019/scpc_2019_codebook.pdf)

Foster, K., Greene, C., & Stavins, J. (2020, June 16). The 2019 Survey of Consumer Payment Choice: Summary Results. Retrieved September 26, 2021, from [https://doi.org/10.29338/rdr2020-03.](https://doi.org/10.29338/rdr2020-03)

