# AV-ecommerce-analytics

AnalyticsVidhya- Gender Prediction for E-Commerce

![Competition banner](images/banner.png)

[Competition Link](https://datahack.analyticsvidhya.com/contest/janatahack-e-commerce-analytics-ml-hackathon/#ProblemStatement)

#### Problem Statement

With the evolution of the information and communication technologies and the rapid growth of the Internet for the exchange and distribution of information, 
Electronic Commerce (e-commerce) has gained massive momentum globally, and attracted more and more worldwide users overcoming the time constraints and 
distance barriers.

It is important to gain in-depth insights into e-commerce via data-driven analytics and identify the factors affecting product sales, the impact of 
characteristics of customers on their purchase habits.

It is quite useful to understand the demand, habits, concern, perception, and interest of customers from the clue of genders for e-commerce companies. 

However, the genders of users are in general unavailable in e-commerce platforms. To address this gap the aim here is to predict the gender of 
e-commerce’s participants from their product viewing records.

#### Dataset Description


- There are three files provided to you, viz train.zip, test.csv and sample_submission.csv which have the following structure.

| Variable	| Definition |
| ------------- | ----------------- |
| session_id	| Session ID |
| startTime | 	Start time of the session |
| endTime	| End Time of the session |
| ProductList | List of products viewed | 
| gender | (Target) male/female | 

- Product list contains list of products viewed by the user in the given session and it also contains the category, sub category, 
sub-sub category and the product all encoded and separated with a slash symbol. Each consecutive product is separated with a semicolon.

#### Evaluation Metric
Submissions are evaluated on accuracy between the predicted and observed gender for the sessions in the test set.

#### Public and Private Split
Test sessions are further divided into Public (40%) and Private (60%)


#### Approach

- Feature engineering of the category, product list
- Feature engineering from the time variables
- 4 K-fold models have been used for training (Randomforest, XGB, LGBM, GBM)


