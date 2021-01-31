# Elo_Merchant
Case Study: Elo Merchant Category Recommendation , Help understand customer loyalty
<h1> 1. Business Problem </h1>
<h3> 1.1 Description </h3>
<p>Elo is one of the biggest and most relaible payment brand in brazil, It planned a reward program to attract the customers based on customers loyalty score.
<h3> 1.2 Problem statement </h3>
<p>Elo wants to predict customers' loyalty based on the given features so they can give more offers to loyal customers which will be in favour of customers and merchants as well. (so they can target individual customers and avoid unnecessary campaigns).
<p>It seems like a recommendation but here we have to predict customers’ loyalty score which is nothing but real value. So this is problem of regression</p>
<h3> 1.3 Sources/Useful Link/Credits </h3>
 Source: https://www.kaggle.com/c/elo-merchant-category-recommendation/overview <br>
https://www.kaggle.com/praxitelisk/elo-eda-ml<br>
https://www.kaggle.com/pedroforli/elo-data-engineering   <br>
https://www.kaggle.com/c/elo-merchant-category-recommendation/discussion/82127<br>
https://www.kaggle.com/batalov/making-sense-of-elo-data-eda<br>
https://www.kaggle.com/mfjwr1/simple-lightgbm-without-blending<br>
<h3>1.4 Real world/Business Objectives and Constraints </h3>
<ol>
<li> No strict latency concerns.
</ol>
<h1>2. Machine Learning Problem </h1>
<h3> 2.1 Data </h3>
Download Data From: https://www.kaggle.com/c/elo-merchant-category-recommendation/data
Total there are 6 files given in data.
<ul>
<li>Data_dictionary.xslx: Description of all columns given in csv files
<li>train.csv :  Training set(contains card_id, feature1, feature2, feature3, first_active_month, target)
<li>test.csv : Testing set.
<li>historical_transactions.csv : upto 3 months historical data for each card id.
<li>merchants.csv : additional merchants information 
<li>new_merchant_transactions: contains transactions at new merchants.
</ul>
<h3> 2.2 Mapping the real world problem to an ML problem </h3>
<h4> 2.2.1 Type of Machine Leaning Problem </h4>
<p>It is regression problem. For given card_id we need to predict loyalty score.
<h4> 2.2.2 Performance Metric </h4>
Source: https://www.kaggle.com/c/elo-merchant-category-recommendation/overview/evaluation

Metric(s): 
* Root Mean Squared Error (RMSE)
