# Isolation Forest Model and LOF for Anomaly Detection in Python

# Project Description

# Business Objective

In the Banking or payment industry, fraud is an illegal usage of credit card details without the real cardholder’s knowledge. A stolen credit card/card number is usually the cause of a fraudulent charge. Once a cardholder sees a payment transaction, he did not make on his credit card statement, he/she has the right to dispute the charge by contacting his/her bank. The bank or Credit Card Company conducts an investigation and returns the money to the cardholder.

But what if we can detect fraudulent transaction activity in real-time? This way we can take the required action to stop the same. We can use machine learning techniques to detect fraudulent transactions. We can use supervised or unsupervised methods of learning depending upon the dataset. For this project, we will be opting for unsupervised learning using Isolation Forest and Local Outlier Factor (LOF) algorithms.

Isolation Forests are similar to Random forests that are built based on decision trees. There are no pre-defined labels here and hence it is an unsupervised algorithm. It was built based on the fact that anomalies or outliers are the data points that are “few and different.” In an Isolation Forest, randomly sub-sampled data is processed in a tree structure based on randomly selected features. The sub-samples that travel deeper into the tree are less likely to be anomalies as they required more cuts to isolate them. The ones which ended up in shorter branches indicated anomalies as it was easier for the tree to separate them from other observations.

Local Outlier Factor or LOF is an unsupervised ML algorithm that identifies outliers with respect to the local neighborhoods as opposed to using the entire data distribution. The advantage of using a LOF is identifying points that are outliers relative to a local cluster of points. This algorithm is based on a concept of local density, where locality is given by k nearest neighbors, whose distance is used to estimate the density.

 
# Data Description

The dataset that we will use for this project consists of 15 numerical columns with 140000 rows which are a result of PCA transformation. These numerical values are nothing but masked credit card transactions. We do not have any background information on the features due to confidentiality reasons.

# Goal

To build a model that is able to correctly identify fraudulent credit card transactions from the valid transactions using Isolation Forest and Local Outlier Factor.


# Tech Stack

- Language - Python
- Libraries - sklearn, pandas, matplotlib, numpy, seaborn

# Approach

- Importing the required libraries and packages
- Open the config.ini file. (This is a configuration file that can be edited according to your dataset)
- Read the dataset (audio files)
- Perform exploratory data analysis
- Handle Missing Values
- Find contamination amount
- Model Training
- Making predictions

# Snapshot

![Screenshot 2023-09-14 at 22 01 26](https://github.com/redjules/isolation-forest-model/assets/106017493/2ec7998b-e0f4-47e0-8491-640fda26f145)

![Screenshot 2023-09-14 at 22 03 20](https://github.com/redjules/isolation-forest-model/assets/106017493/4ebd52f6-35be-4638-a075-004f4b985558)
