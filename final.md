---
title: Detecting Phishing Websites
date: "May 2022"
author: Reshma Parakkal, Santhosh Bodla, Surbhi Dogra, Tanya Gupta, San José State University

header-includes: |
  \usepackage{booktabs}
  \usepackage{caption}
---

# Abstract

Phishing is a dangerous threats to your online accounts and data, because it peretends to be a legitimate source, and incorporates social engineering to make victims
to fall for the attack. In order to prevent phishing attack we aim  to predict the data based on the URL of the website. In this project first we have preformed data preprocessing to clean the data
and then impute the missing values. Later the Discovery of malicious websites is performed by using algorithms like logistic regression, XGBoost, Random Forest and their performance will be evaluated
before and after parameter tuning.

# Introduction
Phishing is a technique used by phishers to steal the user’s confidential and sensitive data, which could lead to financial loss for any individual or organization. Phishing is a serious security problem in the cyber-world and is an illegal act done by the attackers to steal personal identity data and financial account credentials from web users. Phishing sites lure victims to surf on a fake website and steal their confidential data. Due to this reason, research has been conducted to detect and prevent phishing attacks, where models are constructed for performing classification on phishing websites.
We will be incorporating classification models, whose input will be URL attributes. This model will be trained with the exhaustive dataset to maximum accuracy. The dataset includes two dataset with 58,645 and 88,647 website’s URL deemed as fraudulent or real. The website is identified by its attributes which are fed to classification models for classification.
  
   
# Data Description
The data used has been gathered to develop and analyze different classifiers for detecting phishing websites using URL characteristics, URL resolving metrics and external services. Six groups of 
attributes can be found in the prepared dataset:\
  • Item attributes based on the whole URL properties.\
  • Item attributes based on the domain properties\
  • Item attributes based on the URL directory properties.\
  • Item attributes based on the URL file properties.\
  • Item attributes based on the URL parameter properties.\
  • Item attributes based on the URL resolving data and external metrics.
  
 As evident from picture below, the first group is based on the values of the characteristics on the entire URL string, but the values of the next four groups are based on sub-strings. The
last set of attributes is based on URL's resolve metrics as well as external services like Google's search index.

![image](https://user-images.githubusercontent.com/90728105/167979436-fcd7ba8f-8a1d-4a4f-9162-90fcc1443008.png)

This dataset has 111 features in total, except the target phishing attribute, which indicates if the instance is legitimate (0) or phishing (1). the dataset has two versions of the 
dataset, one with 58,645 occurrences with a more or less balanced balance between the target groups, with 30,647 instances categorized as phishing websites and 27,998 
instances labeled as legitimate. The second dataset has 88,647 cases, with 30,647 instances tagged as phishing and 58,000 instances identified as valid, with the goal of simulating a 
real-world situation in which there are more legitimate websites present. We have used dataset small for further analysis and model building as it has more balanced classes.
 
 ![image](https://user-images.githubusercontent.com/90728105/167975120-764f9474-f59b-4044-ab89-a44287ca6433.png)

# Methods

## Data Preprocessing



Visualization-
- Based on co-relation between attributes - we can see few attributes where the value is 1 in heatmap, strongly affect each other. For eg. qty_dot_directory and  qty_hyper_directory are strongly related.
![image](https://user-images.githubusercontent.com/90728105/167982711-845f3513-2fe7-41f8-ba22-df98429f959d.png)

- Before imputation-
 1. Based on nullity in attributes - we can see the attributes like time_domain_expiration, time_domain_activation has maximum amount of missing values and hence, there bar length in green color is shortest in comparison to the length of other attributes.
![image](https://user-images.githubusercontent.com/90728105/167983099-0a990332-8f99-41a7-af1a-eb28c0a19aa4.png)

After Imputation-
- Below we can see after applying each type of imputation we have imputed/substituted the missing value with mean, median and mode. Therefore, all the green bars in the plots are of equal length and are of equal length.
1. Median Imputed\
![image](https://user-images.githubusercontent.com/90728105/167984027-e25f0024-5fb0-4b2d-ba2b-99e61c2519c1.png)
2. Mean Imputed\
![image](https://user-images.githubusercontent.com/90728105/167984332-7a69a27a-1833-4b2e-8309-470d056bdff6.png)
3. Mode Imputed\
![image](https://user-images.githubusercontent.com/90728105/167984112-0e5a96d8-b675-4794-acba-1750056146a2.png)
