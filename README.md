# Churn-Prediction-for-online-shopping-portal
# summary
Engineered a classification and segmentation framework leveraging behavioral and transactional data (161 entries, 40 features) collected via a custom-designed Google Forms survey. Spearheaded exploratory data analysis and feature engineering, optimized imbalanced datasets with RandomOverSampler, and implemented dimensionality reduction (LDA) to enhance model accuracy. Boosted churn class recall to 83% and achieved an AUC of 0.929 using Logistic Regression. Strategically segmented customers into three clusters with K-means based on satisfaction and complaints, and deployed RFM analysis (weights: 0.15/0.28/0.57) to classify customers into five actionable categories. Delivered data-driven retention strategies that empowered targeted decision-making and customer engagement
# Detailed steps
Objective:
Develop a predictive model for customer churn using behavioral and transactional data, providing actionable insights for retention strategies.
 

1.	Data Collection:
    o	Designed a questionnaire via Google Forms.
    o	Collected 161 entries across 40 parameters related to customer behavior and platform usage.
2.	Exploratory Data Analysis (EDA):
    o	Performed univariate, bivariate, and multivariate analysis.
    o	Evaluated correlations between numerical variables and associations between categorical variables using Cramér’s V.
3.	Clustering Analysis:
    o	  Implemented K-Means Clustering to segment customers into 3 clusters based on:
        	Satisfaction scores.
        	Complaints made in the past year.
   o	Validated clusters using the silhouette score and elbow method.
4.	Imbalance Handling:
   o	Managed data imbalance (small churn class) using RandomOverSampler.
5.	Dimensionality Reduction:
   o	Applied Linear Discriminant Analysis (LDA) to reduce features to 1 component, optimizing for class separability.
6.	Modeling:
   o	Tested multiple machine learning models, evaluated using AUC, precision, recall, and other metrics.
   o	Performed cross-validation to ensure no overfitting.
7.	Hypothesis Testing:
   o	Conducted Chi-square tests to validate significant relationships between categorical variables.
 
Model Comparison Table:
Model	                Train AUC      	Test AUC	          Accuracy (Test)  	  Precision (Churn)	    Recall (Churn)
Logistic Regression	    0.883	          0.929	                    90%	            62%	                  83%
Decision Tree	          1.000	          0.790	                    88%	            57%	                  67%
Random Forest	          1.000	          0.898	                    88%	            57%	                  67%
Balanced Random Forest	1.000	          0.902	                    88%	            57%	                  67%
K-Nearest Neighbors	    0.993	          0.840	                    73%	            33%	                  83%


