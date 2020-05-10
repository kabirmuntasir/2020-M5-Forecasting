# 2020-M5-Forecasting 
## https://www.kaggle.com/c/m5-forecasting-uncertainty

## Objectives
The objective of the M5 forecasting competition is to advance the theory and practice of forecasting by identifying the method(s) that provide the most accurate point forecasts for each of the 42,840 time series of the competition. I addition, to elicit information to estimate the uncertainty distribution of the realized values of these series as precisely as possible. 
To that end, the participants of M5 are asked to provide 28 days ahead point forecasts (PFs) for all the series of the competition, as well as the corresponding median and 50%, 67%, 95%, and 99% prediction intervals (PIs).
The M5 differs from the previous four ones in five important ways, some of them suggested by the discussants of the M4  competition, as follows:
 - First, it uses grouped unit sales data, starting at the product-store level and being aggregated to that of product departments, product categories, stores, and three geographical areas: the States of California (CA), Texas (TX), and Wisconsin (WI).
  - Second, besides the time series data, it includes explanatory variables such as sell prices, promotions, days of the week, and special events (e.g. Super Bowl, Valentine’s Day, and Orthodox Easter) that typically affect unit sales and could improve forecasting accuracy.
 - Third, in addition to point forecasts, it assesses the distribution of uncertainty, as the participants are asked to provide information on nine indicative quantiles.
 - Fourth, instead of having a single competition to estimate both the point forecasts and the uncertainty distribution, there will be two parallel tracks using the same dataset, the first requiring 28 days ahead point forecasts and the second 28 days ahead probabilistic forecasts for the median and four prediction intervals (50%, 67%, 95%, and 99%).
 - Fifth, for the first time it focuses on series that display intermittency, i.e., sporadic demand including zeros.

### Dates and hosting
The M5 will start on March 2, 2020 and finish on June 30 of the same year. The competition will be run using the Kaggle platform. Thus, we expect many submissions from all types of forecasters including data scientists, statisticians, and practitioners, expanding the field of forecasting and eventually integrating its various approaches for improving accuracy and uncertainty estimation.

The competition will be divided into two separate Kaggle competitions, using the same dataset, with the first (M5 Forecasting Competition – Accuracy) requiring 28 days ahead point forecasts and the second (M5 Forecasting Competition – Uncertainty) 28 days ahead probabilistic forecasts for the corresponding median and four prediction intervals (50%, 67%, 95%, and 99%).

In order to support the participants to validate their forecasting approaches, the competition will include a validation phase that will take place from March 2, 2020 to 31 May of the same year. During this phase, the participants will be allowed to train their forecasting methods with the data initially provided by the organizers and validate the performance of their approaches using a hidden sample of 28 days, not made publicly available. By submitting their forecasts at the Kaggle platform (a maximum of 5 entries per day), the participants will be informed about the score of their submission, which will be then published in Kaggle’ s real-time leaderboard. Given this instant feedback, participants will be allowed to effectively revise and resubmit their forecasts by learning from the received feedback.

After the end of the validation phase, i.e., from June 1, 2020 to 30 June of the same year, the participants will be provided with the actual values of the 28 days of data used for scoring their performance during the validation phase. They will be asked then to re-estimate or adjust (if needed) their forecasting models in order to submit their final forecasts and prediction intervals for the following 28 days, i.e., the data used for the final evaluation of the participants. During this time, there will be no leaderboard, meaning that no feedback will be given to the participants about their score after submitting their forecasts. Thus, although the participants will be free to (re)submit their forecasts any time they wish (a maximum of 5 entries per day), they will not be aware of their absolute, as well as their relative performance. The final ranks of the participants will be made available only at the end of competition, when the test data will be made available. This is done in order for the competition to simulate reality as closely as possible, given that in real life forecasters do not know the future. 

Note that the submission system will be open from the beginning of the competition, meaning that participants will be able to submit their final forecast from March 2, 2020 to June 30, 2020, even during the validation phase. However, as previously mentioned, the complete M5 training sample (including the 28 days used for the validation phases’ leaderboard) will only become available on June 1, 2020. So, any participant submitting his/his/their final forecasts during the validation phase will be missing the last 28 days of the complete training sample.

Note also that M5 will be divided into two tracks, one requiring point forecasts, and one requiring the estimation of the uncertainty distribution, each with its separate prizes of $50,000. Thus, two individual competitions will be visible at the Kaggle platform, each one with its own separate leaderboard. Participants are allowed to compete and be eligible for prizes in the first track, the second track, or both. 

## The dataset
The M5 dataset, generously made available by Walmart, involves the unit sales of various products sold in the USA, organized in the form of grouped time series. More specifically, the dataset involves the unit sales of 3,049 products, classified in 3 product categories (Hobbies, Foods, and Household) and 7 product departments, in which the above-mentioned categories are disaggregated.  The products are sold across ten stores, located in three States (CA, TX, and WI). In this respect, the bottom-level of the hierarchy, i.e., product-store unit sales can be mapped across either product categories or geographical regions, as follows:
Table 1: Number of M5 series per aggregation level.
Level 
id	Aggregation Level	Number of series
1	Unit sales of all products, aggregated for all stores/states	1
2	Unit sales of all products, aggregated for each State	3
3	Unit sales of all products, aggregated for each store 	10
4	Unit sales of all products, aggregated for each category	3
5	Unit sales of all products, aggregated for each department	7
6	Unit sales of all products, aggregated for each State and category	9
7	Unit sales of all products, aggregated for each State and department	21
8	Unit sales of all products, aggregated for each store and category	30
9	Unit sales of all products, aggregated for each store and department	70
10	Unit sales of product x, aggregated for all stores/states	3,049
11	Unit sales of product x, aggregated for each State	9,147
12	Unit sales of product x, aggregated for each store	30,490
Total	42,840 


For more information
# https://mofc.unic.ac.cy/m5-competition/ 