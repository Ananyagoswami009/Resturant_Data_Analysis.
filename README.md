📊 Restaurant Data Analysis Project
An End-to-End Analytics and Machine Learning Pipeline for Restaurant Intelligence

This repository presents a complete data science project structured into three progressive phases, focused on unlocking business insights and predictive intelligence from a real-world restaurant dataset. The project integrates exploratory data analysis, feature engineering, statistical modeling, customer behavior analytics, and advanced machine learning techniques to address strategic questions in the food services domain.

🔍 Level 1: Exploratory Data Analysis (EDA) & Data Preprocessing
The objective of this phase is to assess data quality, identify patterns, and prepare the dataset for downstream analytics.

✅ Key Activities:
Data Profiling: Analyzed 9551 records across 21 attributes, covering geographic, operational, and customer-related metrics.

Missing Value Treatment: Replaced null values in the 'Cuisines' column with "Unknown" to preserve analytical consistency.

Data Type Validation: Ensured appropriate usage of numerical and categorical data types without requiring transformations.

Target Variable Exploration: Investigated class imbalance in the "Aggregate Rating" variable, noting high concentration around ratings 3.0–4.0 and significant presence of unrated entities.

Descriptive Analytics: Produced statistical summaries (mean, median, std dev) for cost and votes to evaluate central tendencies and dispersion.

📍 Geospatial Visualization:
Developed interactive heatmaps to visualize rating clusters across major cities.

Identified high-density zones and potential rating blind spots (0.0 ratings), highlighting strategic opportunities for restaurant visibility enhancement.


🧩 Level 2: Feature Correlation & Behavioral Analysis
This phase dives into the relationships between restaurant features and their impact on customer satisfaction.

🧠 Feature-Based Insights:
Table Booking: Only 12.12% of restaurants offer it, yet these receive significantly higher ratings (avg: 3.44 vs 2.56). Strong ROI on customer convenience investment.

Online Delivery: Predominantly adopted by budget restaurants (Price Range 1), with a declining presence in premium establishments.

Price Range Dynamics: Clear positive correlation between price tier and average rating—premium restaurants (Range 4) score avg. 3.82 vs. 2.91 for budget ones.

🛠 Feature Engineering:
Created new features like Restaurant Name Length and Address Length to analyze naming strategies and address complexity.

Binary encoding for service-related features (Has Table Booking, Has Online Delivery) to enhance compatibility with ML algorithms.


🤖 Level 3: Predictive Modeling, Customer Segmentation & Advanced Visualizations
This phase focuses on building and comparing machine learning models to predict restaurant ratings and understand customer preference patterns.

🔬 Machine Learning Models Implemented:
Baseline Models: Linear Regression, Ridge, Lasso

Tree-Based Models: Decision Tree, Random Forest, Gradient Boosting, AdaBoost, XGBoost

Others: Support Vector Regression (SVR), K-Nearest Neighbors (KNN)

🏆 Best Model:
Gradient Boosting Regression outperformed others with the lowest Mean Squared Error and highest R² score, successfully capturing non-linear feature interactions.

📊 Customer Behavior Analysis:
Cuisine Popularity: North Indian, Chinese, Italian ranked highest in vote count.

Highly Rated Cuisines: Western and vegetarian cuisines received higher average satisfaction scores despite lower popularity.

Votes vs. Rating Correlation: Weak negative correlation—high engagement doesn't always translate to high satisfaction.

📈 Data Visualizations:
Histogram of Rating Distribution revealed a mid-range concentration (~3.0–4.0), signaling competitive parity.

Scatter Plots & Bar Charts to decode relationships between price, votes, and satisfaction across cuisines and regions.



🎯 Strategic Recommendations
Based on multi-level analysis and model outcomes, the following recommendations are proposed for stakeholders in the restaurant industry:

Expand High-Impact Services: Boost adoption of table booking and online delivery to enhance customer convenience and ratings.

Leverage Premium Positioning: Maintain quality control in higher-priced segments where expectations are elevated.

Promote Underrated Cuisines: Tap into niche markets by elevating highly rated but underrepresented cuisine types.

Focus on Regional Optimization: Use geospatial insights to tailor offerings by city and locality preferences.

Prepare for Predictive Deployment: Engineered features and encoded variables are ML-ready, allowing integration into production-grade recommendation or feedback systems.



🧰 Tech Stack & Tools
Programming Language: Python

Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost, plotly

Machine Learning: Regression Models (Linear, Tree-based, Ensemble), Feature Engineering, Hyperparameter Tuning

Data Visualization: Heatmaps, Bar Plots, Histograms, Scatter Plots

Data Preparation: Null handling, One-hot/Binary encoding, Data normalization

Deployment Readiness: Dataset is preprocessed and enriched for direct use in ML pipelines and BI tools.
