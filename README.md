# smartphone_analysis

#🔗 Live Demo → myracorreia05.github.io/smartphone-analysis

📌 Project Overview
This project applies a full data science pipeline to primary survey data collected from 1,200 smartphone users. It uncovers patterns in OS preference, switching behavior, feature priorities, and user psychology — culminating in an interactive single-file HTML dashboard with 6 analytical tabs, 15+ charts, and ML results.

🔬 What's Inside

Python Analysis (smartphone_analysis_deep.py)
StageTechniqueData Wranglingpandas · feature engineering · ordinal encodingExploratory AnalysisDistribution plots · violin · boxplots · crosstabsHypothesis TestingMann-Whitney U · Pearson r · Point-biserial rDimensionality ReductionPCA (2 components, ~55% variance explained)ClusteringK-Means (k=4, Elbow method)ClassificationRandom Forest · Gradient Boosting · Logistic Regression · SVMModel Evaluation5-fold Stratified CV · ROC-AUC · Feature ImportanceVisualizationmatplotlib · seaborn · radar chart · heatmaps
Interactive Dashboard (index.html)

6 tabs: Overview · Feature Analysis · Statistics · ML & Clustering · Demographics · Key Insights
15+ Chart.js visualizations — doughnuts, grouped bars, scatter plots, line charts, ROC curves, radar charts
Zero dependencies — single file, opens in any browser, no server needed
Fully responsive — works on mobile and desktop


📊 Key Findings

🔗 Ecosystem is Apple's #1 retention driver — iPhone users rate Ecosystem 4.22/5 vs 3.62/5 for Android, the most statistically significant gap in the dataset (p<0.0001) and the top predictor in the Random Forest model.
⚡ Android users are pragmatic power users — Customization (4.28 vs 2.84, p<0.0001) and Battery (4.31 vs 3.87, p=0.04) are significantly higher for Android; 42% of Android users have 100+ apps installed.
❤️ Satisfied users never switch — Pearson r = −0.51 (p<0.001) between satisfaction and switch likelihood. Users scoring 5/5 satisfaction have a switch likelihood of just 1.2/5.
🔄 Switcher asymmetry is 2.8× — 512 users moved Android→iPhone vs only 184 iPhone→Android, confirming Apple's ecosystem creates a measurable one-way gravity pull.
🤖 ML can predict OS from preferences alone — Random Forest achieves 81% accuracy (5-fold CV) with ROC-AUC = 0.84. Top predictors: Ecosystem, Customization, Brand reputation.
🧩 4 distinct user archetypes discovered — K-Means (k=4, confirmed by Elbow method) reveals Pragmatic Users, Ecosystem Loyalists, Feature Enthusiasts, and Budget Basics — each with distinct OS skew and satisfaction profiles.
🤝 Peer influence has zero effect — Lowest-rated feature across all segments at avg 2.08/5 (p=0.38, not significant). Smartphone choice is entirely self-directed.
💰 Price only matters to Android users — Significant difference at p=0.003. iPhone users are measurably price-insensitive, confirming Apple's ability to sustain premium pricing without churn risk.
