# yelp-rating-prediction
Predicting Consumer Ratings and Analyzing Popularity Drivers: An Integrated Analysis of Restaurant Features and Review Text on Yelp

Code and data for Yelp restaurant rating prediction study

This repository contains the code and processed data supporting our paper "Predicting Yelp Restaurant Ratings with Machine Learning and Business Clustering".
Accurately predicting restaurant ratings is challenging due to the interplay of sentiment, operational features, user engagement, and local economic contexts. Our framework integrates prediction and clustering, combining Yelp’s open dataset (business, reviews, check-ins) with BEA per capita income data.
##Key contributions:
###Feature Engineering:
Sentiment analysis (VADER, BERT)
SMOGN for imbalanced rating distribution
PCA for dimensionality reduction
###Modeling:
Baselines: Ridge, Random Forest
Advanced: LightGBM, XGBoost, stacked LightGBM–MLP, stacked XGBoost-Ridge
###Results:
Best model: R² ≈ 0.75, RMSE ≈ 0.42, >81% accuracy (±0.5)
Outperforms single-model baselines (LightGBM R² ≈ 0.65; Ridge R² ≈ 0.58)
###Business Clustering (K-means):
High-end restaurants rely on social engagement
Family-style restaurants emphasize convenience
Fast-food outlets focus on efficiency
##Data:
Original data: Yelp Open Dataset https://chatgpt.com/c/68cf8262-2920-8328-bac9-8d62566d8577#:~:text=Original%20data:%20Yelp-,Open,-Dataset
Processed features (environment, taste, service quality scores) are Final_real.csv. 

This work provides both a reproducible framework for platform-based restaurant analysis and actionable insights for restaurateurs.
