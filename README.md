# CMPE 255: Term Project Proposal Spring 2022 

## Team Members(Group 11):

- Reshma Parakkal(015326454)
- Santhosh Bodla(016002454)
- Surbhi Dogra (015569723)
- Tanya Gupta(014748799)

## Project Title : [Detecting Phishing Websites](https://data.mendeley.com/datasets/72ptz43s9v/1)
 
## Data Set: Phishing Websites Dataset

These data consist of a collection of legitimate as well as phishing website instances. Each website is represented by the set of features which denote whether the website is legitimate or not. Data can serve as an input for the machine learning process.
There are two variants in Phishing datasets provided:
Full Variant : 88,647 instances with 111 features
Small Variant : 58,645 instances with 111 features

## Description of the problem:

### What is Phishing?
Phishing is a kind of social engineering assault that is frequently used to obtain sensitive information from users, such as login passwords and credit card details. It happens when a hacker poses as a trustworthy entity and convinces a victim to access a webpage, email, instant chat, or text message. The receiver is subsequently duped into clicking a malicious link, which can result in malware installation, system freeze as part of a ransomware assault, or the disclosure of sensitive information.

People are the most common targets of web attackers that want to steal their personal information. Hackers try to replicate the original website in order to take advantage of the user. The user believes the website is authentic, but it is not. When a user enters their credentials on a phishing site, the information is transmitted to the attackers' servers, where they can steal credit card information, personal information, or even implant malware on the victim's laptop. As the number of online transactions increases, so does one's vulnerability to these attacks.
Potential Methods:
To reduce the number of assaults leading to bogus websites, we suggest an approach that uses data mining algorithms to detect harmful websites by tracking down the URL.To imitate a legitimate website, attackers modify the subdomain and file path (if it appears in the URL) or make a typographical error. As a result, we must examine the URL and determine what each element includes in order to detect phishing websites. We plan to use Supervised Learning models like Decision Trees, Support Vector Machines(SVM), Naive Bayes Classifier and Random Forest are examples of potential techniques. We intend to introduce some more ways if we go farther into the project.

We are using **Logistic Regression** because it can be useful in identifying the phishing website instances because it gives the discrete outcome on the dataset. In our case, whether the url is malicious or not.

**SVM or support vector machine** is a kind of supervised learning model with algorithms which are used to analyze data for classification and regression analysis. SVM will help us in identifying the phishing websites from the given dataset by building a model which will map training examples to points in space to maximize the width of the gap between the two categories.

**Naive Bayes** is a kind of classifier that works on the Bayes theorem. Prediction of membership probabilities is made for every class such as the probability of data points associated with a particular class.

**The XGBoost, or Extreme Gradient Boosting** method is a decision tree-based machine learning algorithm that improves performance through a process known as boosting. Gradient Boosting Decision Trees (GBDT) is a decision tree ensemble learning algorithm for classification and regression that is similar to random forest. To create a better model, ensemble learning techniques combine different machine learning algorithms, basically GBDT???s train an ensemble of shallow decision trees iteratively, with each iteration using the prior model's error residuals to fit the next model. The final prediction is a weighted sum of all of the tree predictions. In general Random forest ???bagging??? minimizes the variance and overfitting, while GBDT ???boosting??? minimizes the bias and underfitting.

XGBoost is a scalable and highly accurate version of gradient boosting that pushes the limits of computing power for boosted tree algorithms. It was designed primarily to increase machine learning model performance and computational speed. With XGBoost, trees are built in parallel, instead of sequentially like GBDT. It follows a level-wise strategy, scanning across gradient values and using these partial sums to evaluate the quality of splits at every possible split in the training set. 


**Random Forest** is a tree-based ensemble learning algorithm. It is a collection of decision trees derived from a subset of the training data chosen at random. It combines the votes from various decision trees to determine the test object's final class.


Our project's purpose is to discover the most accurate data mining algorithm in order to identify a ???fake website??? that takes personal information 
from consumers.





