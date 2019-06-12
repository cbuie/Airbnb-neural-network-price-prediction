# Module 4 final project: predicting Airbnb prices with machine learning and deep learning

## Introduction and project aims

Airbnb is a home-sharing platform that allows home-owners and renters ('hosts') to put their properties ('listings') online, so that guests can pay to stay in them. Hosts are expected to set their own prices for their listings. Although Airbnb and other sites provide some general guidance, there are currently no free services which help hosts price their properties. Paid third party pricing software is available, but generally you are required to put in your own expected average price ('base price'), and the algorithm will vary the daily price around that base price on each day depending on day of the week, seasonality, how far away the date is, and other factors.

Airbnb pricing is important to get right, particularly in big cities like London where there is lots of competition and even small differences in prices can make the difference between optimum occupancy and high earnings, or being priced out of the market. It is also a difficult thing to do correctly, in order to balance the price with occupancy (which varies inversely with price) in order to maximise revenue.

This project aims to use machine learning and deep learning to predict the base price for properties in London, and also to explore Airbnb listing data, in order to help Airbnb hosts maximise their earnings.

Additional context: I previously worked for a year and a half at an Airbnb property management company, as head of the team responsible for pricing, revenue and analysis. Decisions made during the course of this project are therefore informed by domain expertise in this industry.

I wrote a three-part blog mini-series on this project for Towards Data Science:
- [Part 1](https://towardsdatascience.com/predicting-airbnb-prices-with-deep-learning-part-1-how-to-clean-up-airbnb-data-a5d58e299f6c?source=friends_link&sk=0ad5a63e68210846c65f231826921a00) described some of the more interesting difficulties I faced in cleaning the data - specifically in dealing with messay location and text data
- [Part 2](https://towardsdatascience.com/predicting-airbnb-prices-with-deep-learning-part-2-how-to-improve-your-nightly-price-50ea8bc2bd29?source=friends_link&sk=dfa75bf21a5f2886d2a38f9bdca1f351) presented the results of the exploration of London Airbnb price data, including suggestions for how Airbnb hosts could help boost their listing's earnings
- [Part 3](https://towardsdatascience.com/predicting-airbnb-prices-with-machine-learning-and-deep-learning-f46d44afb8a6?source=friends_link&sk=d380dccd3606a025df173598bae3b445) explained the modelling process, including a walkthrough of the machine learning (XGBoost) and deep learning (multi-layer perceptron/neural network) models produced, and the results of the modelling


## Conclusions

Overall, after experimenting with various machine learning and deep learning models, the best model was an XGBoost model, which was able to explain 73% of the variation in price. The remaining 27% is probably made up of features that were not present in the data. It is likely that a significant proportion of this unexplained variance is due to variations in the listing photos. The photos of properties on Airbnb are very important in encouraging guests to book, and so can also be expected to have a significant impact on price - better photos (primarily better quality properties and furnishings, but also better quality photography) equal higher prices.