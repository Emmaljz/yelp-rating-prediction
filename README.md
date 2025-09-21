# yelp-rating-prediction
Predicting Consumer Ratings and Analyzing Popularity Drivers: An Integrated Analysis of Restaurant Features and Review Text on Yelp

Code and data for Yelp restaurant rating prediction study

This repository contains the code and processed data supporting our paper "Predicting Yelp Restaurant Ratings with Machine Learning and Business Clustering".
Accurately predicting restaurant ratings is challenging due to the interplay of sentiment, operational features, user engagement, and local economic contexts. Our framework integrates prediction and clustering, combining Yelp’s open dataset (business, reviews, check-ins) with BEA per capita income data.

## Key contributions:

### Feature Engineering:
Sentiment analysis (VADER, BERT)
SMOGN for imbalanced rating distribution
PCA for dimensionality reduction

### Modeling:
Baselines: Ridge, Random Forest
Advanced: LightGBM, XGBoost, stacked LightGBM–MLP, stacked XGBoost-Ridge

### Results:
Best model: R² ≈ 0.75, RMSE ≈ 0.42, >81% accuracy (±0.5)
Outperforms single-model baselines (LightGBM R² ≈ 0.65; Ridge R² ≈ 0.58)

### Business Clustering (K-means):
High-end restaurants rely on social engagement
Family-style restaurants emphasize convenience
Fast-food outlets focus on efficiency

## Data:
Original data: Yelp Open Dataset https://business.yelp.com/data/resources/open-dataset/
Processed features (environment, taste, service quality scores) are Final_real.csv. 

This work provides both a reproducible framework for platform-based restaurant analysis and actionable insights for restaurateurs.

## Author:
Li Jiazhou 1a*, Liu Zihao 1b*
1a Hainan International College, Communication University of China, Beijing 100024, China, 202429033112n@mails.cuc.edu.cn
2b International Business School Suzhou (IBSS), Xi’an Jiaotong-Liverpool University, Suzhou 215123, China, Zihao.Liu22@student.xjtlu.edu.cn
<img width="432" height="100" alt="image" src="https://github.com/user-attachments/assets/fa6e8821-6b04-4faf-93e3-d5756de595e5" />

