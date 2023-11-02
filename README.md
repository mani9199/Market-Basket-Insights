**Market-Basket-Insights**

INTODUCTION

Market Basket Analysis is a modelling technique based upon the theory that if you buy a certain group of items, you are more or less likelMarket basket analysis scrutinizes the products customers tend to buy together, and uses the information to decide which products should be cross-sold or promoted together. The term arises from the shopping carts supermarket shoppers fill up during a shopping trip.y to buy another group of items. Market basket analysis may provide the retailer with information to understand the purchase behavior of a buyer. This information can then be used for purposes of cross-selling and up-selling, in addition to influencing sales promotions, loyalty programs, store design, and discount plans.

Market basket analysis scrutinizes the products customers tend to buy together, and uses the information to decide which products should be cross-sold or promoted together. The term arises from the shopping carts supermarket shoppers fill up during a shopping trip.

Association Rule Mining is used when we want to find an association between different objects in a set, find frequent patterns in a transaction database, relational databases or any other information repository.


PROJECT ORGANISATION

                            
Design	-  contain design of thinking

Innovation creation	                    - These innovative ideas became the driving force behind the project's advancement



Market basket analysis	                - Market Basket Analysis to find products association

Analysis                                - data set

Feature extraction	                    - feature engineering and extraction for a ML model

Model	                                  - neural network model for product reoder prediction

Redme	                                  - project report

DESIGN

Data collection            : Collect sales data, including customer transactions, items purchased, and transaction timestamps.

Data preprocessing    : Remove duplicates, handle missing values, and ensure data consistency.

Rule mining                 : Set minimum support and confidence thresholds to filter out less significant associations.

Reporting                     : Develop a report or dashboard to communicate the insights to stakeholders.

Evaluation                    : Implement a system for continuous data collection and analysis to keep the market basket insights up-to-date and relevant.

INNOVATION CREATION

Building upon the design thinking framework, the project ventured into a phase dedicated to innovative ideation. 
This creative stage was where the project team brainstormed and nurtured ground-breaking concepts to elevate the analysis effectiveness. 

MARKET BASKET ANALYSIS

•	Changing the store layout according to trends

•	Customers behavior analysis 

•	Catalog Design

•	Cross marketing on online stores

•	Customized emails with add-on sales, etc.

ML MODELS

Using the extracted features, I prepared a dataframe which shows all the products user has bought previously, user level features, product level features, asile and department level features, user-product level features and the information of current order such as order's day-of-week, hour-of-day, etc. The Traget would be 'reordered' which shows how many of the previously purchased items, user ordered this time.

Since the dataframe is huge, I reduced the memory consumption of it by downcasting to fit the data int my memory. I preferred MinMaxScaler over StandardScaler as the latter requires 16 GB of RAM for its operation. I followed standard process for model building and I relied on XGBoost as it handles large data, can be parallelized and gives feature importance. I also built Neural Network to see what would be the best performance from this model disregarding some inherent randomness from both of these models. To balance the data, I have used cost-sensitive learning by assigning class weightage (~{0:1, 1:10}). I have not used random-upsampling/SMOTE as it would increase the data size and I do not have much memory. Also, since random-down-sampling discards information which might be important and would result in bias.


![image](https://github.com/Marees1267/Market-Basket-Insights/assets/146077504/daf4c79a-d9aa-44ef-b217-3b1e510ab652)

![image](https://github.com/Marees1267/Market-Basket-Insights/assets/146077504/79acbfaa-f861-4df5-8bfe-05dd494a69e6)

TECHNOLOGIES USED

![image](https://github.com/Marees1267/Market-Basket-Insights/assets/146077504/11bcb8b7-379c-402a-a53f-3c6e807730cf)

![image](https://github.com/Marees1267/Market-Basket-Insights/assets/146077504/1c4f5630-52ff-4897-836f-149c92921112)


CREDITS

•	A huge shout-out to the kaggle dataset 




