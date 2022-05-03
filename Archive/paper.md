---
title: Detecting Phishing Websites
date: "May 2022"
author: Reshma Parakkal, Santhosh Bodla, Surbhi Dogra, Tanya Gupta, San José State University

header-includes: |
  \usepackage{booktabs}
  \usepackage{caption}
---

# Abstract

Pizza [@pizza2000identification] is an understudied yet widely utilized implement for delivering in-vivo *Solanum lycopersicum* based liquid mediums in a variety of next-generation mastications studies. Here we describe a de novo approach for large scale *T. aestivum* assemblies based on protein folding that drastically reduces the generation time of the mutation rate.

# Introduction

# Methods

## Data Preprocessing

Data Preprocessing is referred to as manipulation or dropping of data before it is used to ensure or enhance performance. It is basically the process of transforming the raw data into understandable format. Data preprocessing is the most important phase of  machine learning. It includes removing irrelevant and redundant information from the data. Examples of data preprocessing include cleaning, instance selection, normalization, feature extraction and selection. The product of data preprocessing is the final training set. The dataset that we have selected contained irrelevant and meaningless information which has been removed.

Firstly, we filtered the data by dropping duplicate rows. These values were removed to reduce the dimensionality. 
Next, we analysed that the dataset contained '-1' values throughout where almost all the rows had this value, so we cannot drop all this data. We then checked the percentage of '-1' values in each column. 

As per the previous analysis, we have noticed that almost 80% of the dataset contains ‘-1’. Since most of the columns have ‘-1’, it would not be wise to remove them altogether as they may significantly affect the result. To tackle this, we remove the columns with less than 80% ‘-1’ and replace them with Nan. To improve the efficiency while testing and training, we drop the rest of the columns.

Once we have dropped values containing ‘-1’, the next step is to look at the missing values. There are three main reasons why values could be missing – Missing at random, Missing Completely at random, Not Missing at random. The initial approach initiated for imputing is using mean imputation. As the name suggests, the mean is calculated for the available values and replaced with the non-missing value’s number. An essential step to bear in mind during mean imputation is to remove outliers to prevent seeing absurd or surprising values as mean.

In addition to this, the missing values are also imputed using median and mode. These methods do not necessarily worry about outliers as they work using the middle values that are present when the column values are sorted. The last imputation method used is the most effective in predicting the missing values. It uses the Nearest Neighbor method known as KNN imputation, where the Nan values are replaced with the values of the neighboring values.



## Models to be used

### Logistic Regression 
Logistic regression is a supervised learning technique. It is used to calculate or predict the probability of a binary event occurring. It is used in statistical software to understand the relationship between the dependent variable and one or more independent variables by estimating probabilities using a logistic regression equation. 

### Random Forest Classifier
Random Forest Classifier is used to test and train the data, a supervised machine learning algorithm. The main reason behind picking random forests is to overcome the problem of overfitting. Reducing overfitting is achieved by selecting features randomly compared to decision trees that work only using the rules generated.

# Comparisons

# Example Analysis

# Conclusions


# References
