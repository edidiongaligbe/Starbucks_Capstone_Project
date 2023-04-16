# Udacity Machine Learning Nanodegree Capstone Project

### Introduction
Starbucks offers promotions designed to attract new customers and encourage existing customers to make repeat purchases, building brand loyalty. These promotions could be in
form of loyalty programs, buy one, get one free (BOGO), gift cards, etc. These offers come
through emails, the web, mobile app, and social media. The company keeps a record of
customers’ interactions with these promotions and the data is useful to serve the customer
better based on their activities and preferences.

The aim of sending promotions and offers to customers is to encourage customers to make
purchases. It will not be an intelligent move to send the same promotion to all the
customers at once, this may result in promotions that do not yield the expected results. The
goal of this project is to make use of the data from Starbucks to determine what promotion
to send to a demography of customers that will result in higher customer purchases.


### Data
The data is contained in three files:
1. **profile**.json: Contains demographic data for each customer. It is made up of 17,000 customers with 5 fields.
    * gender: (categorical) M, F, O, or null.
    * age: (numeric) missing value encoded as 118.
    * id: (string/hash).
    * became_member_on: (date) format:YYYYMMDD.
    * income: (numeric).
2. **portfolio.json**: Contains data on offers sent during 30-day test period. It is made up of 10 offers with 6 fields.
    * reward: (numeric) money awarded for the amount spent.
    * channels: (list) web, email, mobile, social.
    * difficulty: (numeric) money required to be spent to receive reward.
    * duration: (numeric) time for offer to be open, in days.
    * offer_type: (string) bogo, discount, informational.
    * id: (string/hash).
3. **transcript.json**: Contains records for customer transactions, offers received, offers viewed, and offers completed. It is made up of 306648 transactions with 4 fields.
    * person: (string/hash).
    * event: (string) offer received, offer.
    * value: (dictionary) different values depending on event type:
        * offer id: (string/hash) not associated with any "transaction".
        * amount: (numeric) money spent in "transaction".
        * reward: (numeric) money gained from "offer completed".
    * time: (numeric) hours after start of test.


### Libraries
1. **AutoGluon**: An autoML open source library for model training.
2. **Pandas**: A Python library that is used to analyze data.
3. **Numpy**: A standard Python library for working with numerical data.
4. **Matplotlib**: a library for creating visualizations in Python.
5. **Seaborn**: A library that uses Matplotlib underneath to plot graphs, it gives a rich visual.


### Evaluation Metrics
The following metrics are used to evaluate the model.
1. Accuracy. 
2. Balanced Accuracy.
3. Matthew Correlation Coefficient (MCC)

### Credits and Acknowledgements
Thanks to Udacity for providing dataset.