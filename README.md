# Udacity Capstone Project: Customer Segmentation

## Introduction

This repository is part of Udacity's Data Science Nanodegree and comprises the code for the final capstone project. The project was about clustering customer data and comparing it to demographica data. 
Furthermore a supervised analysis should be made wheather or nor potentail customers would reply to an email.

## Methology:

The code is mainly divided in three tasks: 

- Code cleaning: The given data was not cleaned and should be prepared for the next two steps.
- Unsupervised learning: Once cleaned the data should be clustered. The clustered customers should then be compared to the demographic clusters.
- Supervised learning: Last but not least given customers data should be used to predict if a customer would reply to a mail.

## Libraries:

The following libraries were used during the project:

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `sklearn`
- `xgboost`
- `pickle`

## Files

Since I am not allowed to share any datasets the repo is comprised of the following files:

- CustomerClsutering
  - ArvatoProject.ipynb
  - README.md
  - LICENSE

## Results and Improvents

Unsupervides clustering ended with identification of 10 clusters, where I used 5 to further investigate what kind of customers are part of the corresponding clusters. It turned mostly out that a high proportion are eldery, relatively wealthy people.

For learning the chance of customer response I chosed XGBoosts since it is known to perform good when the data is highly inbalanced.

The algorithmn shows a AUROC-Score of approx. 75%.

Of course the above score and clustering can further be improved. 

For example the feature engineering part could be extended and improved. With better resources available it would also be possible to use more than two methods to determine the optimal number of clusters.
As a second example one could further optimize the parameters used XGBoost and test other algorithmns which are also well suited for highly imbalanced data.
