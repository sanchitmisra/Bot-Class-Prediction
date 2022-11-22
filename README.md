# Bot-Class-Prediction-

# Problem Description
Build a model to detect Non-Human Traffic Present in a website

## Why do we need to detect Bots ?
No matter how big your website is, you’re almost guaranteed to receive bot traffic at some point. These bots are often up to a range of different things on your site, from indexing web pages to scraping your content. With so many different bots out there, how can you detect bot traffic on your website? And should you be concerned?
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
