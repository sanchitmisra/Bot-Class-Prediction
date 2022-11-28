# Bot-Class-Prediction-
## Tags: Data Science, Machine Learning, Classification, Data Analysis
Summary:
# Problem Description
Build a model to detect Non-Human Traffic Present in a website

![image](https://user-images.githubusercontent.com/99437560/204224629-d17a52a7-29fb-4934-8c96-28e79c79afbe.png)

## Why do we need to detect Bots ?
No matter how big your website is, you’re almost guaranteed to receive bot traffic at some point. These bots are often up to a range of different things on your site, from indexing web pages to scraping your content. With so many different bots out there, how can you detect bot traffic on your website? And should you be concerned?

The purpose of such a predictive model which tries to foresee the bot presence is to combine various econometric parameters that can effectively gauge the website presence of a company and enable the management to take pre-emptive measures that can potentially help to avoid any breakdown distress to the company.

In this project we present our analysis of the data at hand as we go on selecting various subsets of the huge feature space available to us. We try to compile and compare each and every result as we step from a niave modelling to a more nuanced and standard one. We have employed some of the most widely used classification algorithms for this project namely;


Random Forest

Balanced Bagging

Gradient Boosting

Easy Ensemble Technique

We began our analysis by visualizing the sparsity of the two target classes (bot and non-bot) in our dataset. Once we were assured of the huge class imbalance in the data we were going to work on, we began to speculate that the prediction could very well be an anamoly detection problem.

We used box plots to visualize how each feature was distributed over each of the two target classes. This gave us a clear idea as to which variable was contributing more to the bot presence.

As we deep dived into the dataset it become increasingly clear that the classes had a rich overlap and hence could barely be modelled into an class imbalance.

Towards the begining, our approach mainly included reducing the dimensionality of the dataset and getting an ideal number of features which could be modelled with ease and effeciency. We employed some of the most commonly used feature engineering techniques like; Threshold Variance, Information Gain, Random Forest, Lasso and a few others to subset our feature space and remove the ominous curse of dimensionality.

Finally we started the machine learning part on the choosen feature subsets, did cross validation for each of the models' hyperparameters and recorded the performance in each case into a compact dataframe. The evaluation metrics we chose for our project include roc_auc score, f1-score.



# Dataset Description

## Features Description

ctry_name: Indicated from which country user is from

intgrtdmngmtname: team handling the particular domain for the user

intgrtdoperatingteam_name: Operating team name IP is managed from

city: Indicates from which city ip is coming from

st: Indicates from which state ip is coming from

seclvldomn: (.com)(.net) known as secondary domain for example in google.com(.com is secondary domain and google is primary domain)

device_type: From which device ip is operating from

operating_sys: From which operating system ip is coming from

ip_addr: Indicates the user information from where it's operating in the from of unique IP address

user_agent: From which browser version user is operating to any website

VISIT: How many times ip is visited

ENGDVISIT: How ipaddr or user is getting engaged

VIEWS: How many time user has visited the webpage

pageurl: Website Url ipaddress visiting

wk: indicated the week

mth: indicate the month

yr: indicate the year

pagevwts: Giving full info about when and at what time user has visited any website

target: 1 or 0 whether it's an bot or not




"Classification model was created to conduct an analysis that can detect the Non-
Human Traffic presence on website using, Gradient Boosting Classifier & RF."

## Dataset
![image](https://user-images.githubusercontent.com/99437560/203239564-187763ac-0c24-49c1-81bb-830374f180ca.png)
## EDA 
An EDA is a detailed analysis designed to reveal a data set's underlying structure. It is significant for a business because it identifies trends, patterns, and linkages that are not intuitively clear.

![image](https://user-images.githubusercontent.com/99437560/203239937-e503b6d7-eb2a-4c34-bc0a-e8f2b388909e.png)
## Check Outliers
Extreme values that deviate from the majority of other data points in a dataset are known as outliers. They may significantly affect your statistical analysis and distort the outcomes of any hypothesis testing.
![image](https://user-images.githubusercontent.com/99437560/203240368-a25c8347-c161-4382-966e-1f08f52a91b4.png)
## Multicollinearity
A correlation could be positive, meaning both variables move in the same direction, or negative, meaning that when one variable’s value increases, the other variables’ values decrease. Correlation can also be neutral or zero, meaning that the variables are unrelated.
![image](https://user-images.githubusercontent.com/99437560/203240496-2eebe789-23a9-426e-89c9-e519b4dd2455.png)
## Model Building
A computer programme that uses a dataset that has never been seen before to detect patterns or make choices is known as a machine learning model. Model training is the process of using a dataset (referred to as training data) to run a machine learning algorithm and then optimising the algorithm to uncover certain patterns or outputs. The trained machine learning model is the resultant function containing rules and data structures.

![image](https://user-images.githubusercontent.com/99437560/203241040-14078405-54f0-467f-a955-9d9aca8f9ede.png)
# Conclusion
* Engaged visit and views variable are majorly helped us to identify the bots.
* We were able to recognise bots by counting how often each system was accessed.
