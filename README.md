# Akash-Ramanan-Sports-Data-Scientist
Welcome to my portfolio! I’m a Sports Data scientist specialized in sports technical and tactical analysis and biomechanics data with expertise in machine learning, statistics,  and hands-on experience building end-to-end data projects using Python, SQL, PowerBI and Cloud platforms.  


## Projects

### 1. Classification of Elite and sub elite Goalkeepers from professional football using multiple machine learning models (Internship Project)

https://github.com/Ash1708/Classification-of-Goalkeepers_ML/blob/main/README.md

Implemented a machine learning pipeline to classify elite vs. sub-elite goalkeepers using Opta football data. Compared Logistic Regression, Random Forest, and Gradient Boosting models, achieving ~67% accuracy and 0.72 ROC-AUC. Project demonstrates end-to-end ML skills: preprocessing, feature selection (RFE), cross-validation, model evaluation, and feature interpretability — with insights highlighting the importance of distribution and passing skills in modern elite goalkeepers.

* Built ML models to classify elite vs. sub-elite goalkeepers in top European leagues.
* Elite GK = UEFA Champions League appearance (proxy for top-tier status).
* Based on real-world Opta Sports performance data (14,671 match observations).

## Question 
* Which performance attributes best distinguish elite from sub-elite professional football goalkeepers, and can machine learning models reliably classify them based on match performance data?
  
## Libraries & Tools

* Data handling & preprocessing: Pandas, Numpy
* Machine learning & feature selection: Scikit-learn (Logistic Regression, Random Forest, Gradient Boosting, RFE, GridSearchCV, train/test split)
* Visualization: Matplotlib, Seaborn (confusion matrices, ROC curves, feature importance plots)
* Environment: Jupyter Notebook, Python 3.x

 ## Results

* Test accuracy: ~66–67% (similar across all models).
* ROC-AUC: ~0.72, F1 ≈ 0.65.

## Insights: Common features across models (n=15).

* Elite indicators: short distribution, passes received, successful forward passes, clean sheets.
* Sub-elite indicators: long distribution, unsuccessful opposition-half passes, more goals conceded.



## 2. Evaluation of Market Value of Elite Midfielders by Vertical Passing Ability
https://github.com/Ash1708/Evaluation-of-Market-Value-of-Elite-Midfielders-by-Vertical-Passing-Ability/blob/main/README.md

### Research Question

Does the vertical passing performance of elite midfielders correlate with their transfer market value? In other words, this project investigates whether midfielders who play more vertical passes (forward, line-breaking passes) tend to have higher market valuations.

### Hypothesis

Midfielders who consistently play with greater verticality per pass (i.e. higher average forward progression towards goal) are hypothesized to have higher transfer market values. The expectation is that strong forward-passing ability translates into greater player valuation.

### Methodology

* Data: Utilized Opta event data from 282 Ligue 1 matches (2020/21 season), capturing detailed pass events. The transfer market values of players at end of that season were obtained from Transfermarkt.

* Metrics: Defined two novel metrics – verticality and depth – to quantify a midfielder’s vertical passing ability. Verticality measures the forward distance component of passes (how much a pass advances play towards the opponent’s goal on average), while depth measures the effective forward penetration considering angle to goal. These metrics capture how aggressively a player progresses the ball upfield beyond simple pass counts.

### Key Insights

* Vertical Passing vs. Market Value: There is a significant positive correlation between the vertical passing metrics (verticality, depth) and market value for central midfielders – particularly “true” central midfielders and attacking midfielders – indicating that midfielders who excel at forward passes tend to be valued more highly. This correlation is most pronounced among mature players (roughly over 24 years old), who are often in their peak performance years.

* Role and Age Differences: Younger players (especially those under 24) show limited or no correlation between vertical passing performance and market value, suggesting that raw vertical passing ability alone doesn’t drive value in youth. Wing midfielders (wide players) also exhibit weaker and less consistent correlations – their market value often ties more to attributes like pace and crossing rather than vertical passing. In contrast, for mid-career true and offensive midfielders (mid-20s and above), higher verticality/depth strongly correlates with higher market value. (Notably, in the data a strong negative correlation was observed for under-24 offensive mids, indicating that very young attacking midfielders with high verticality were not yet highly valued.)

* Implications for Player Valuation: The metrics verticality and depth show promise as valuable key performance indicators (KPIs) for player valuation. In practice, clubs and analysts could use these vertical passing metrics to identify midfielders who contribute significantly to forward play. The study’s findings suggest these metrics add a useful new dimension to player evaluation, complementing traditional stats. Particularly for players in their prime, strong vertical passing ability is an indicator of higher market worth, underlining that tactical proficiency in advancing the ball vertically is linked to a midfielder’s financial value.




# 3. Sentiment-Analysis-on-IMDB-Reviews (Azure Data Factory + Azure Data Lake + Databricks (PySpark, scikit-learn) + Power BI)
https://github.com/Ash1708/The-Voice-of-the-Audience-Sentiment-Analysis-on-IMDB-Reviews/tree/main

### Project Overview
This project demonstrates how to build a full machine learning pipeline for sentiment analysis, leveraging Azure Databricks for large-scale training and Power BI for business insights. Using the IMDB reviews dataset, I implemented an NLP workflow that classifies movie reviews as positive or negative, and translated model results into actionable insights for decision-making.

### Tech Stack:
* Azure Data Factory, Azure Data Lake, Databricks (PySpark, scikit-learn), Power BI.

Highlights:
* Ingested IMDB dataset into Azure Data Lake and structured raw vs curated zones.
* Trained baseline Logistic Regression NLP model (TF-IDF + Logistic Regression).
* Exported predictions and built a Power BI dashboard with KPIs, confusion matrix, probability histograms, and misclassified reviews.
  
Results: Accuracy ~89%, F1-score ~89%, ROC-AUC ~96%.


Key Insight: Misclassification analysis revealed false positives lead to overestimated satisfaction, guiding customer feedback strategies.
