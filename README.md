# Finlatics-Machine-Learning
This repository, **Finlatics-Machine-Learning**, contains a collection of machine learning projects focused on predictive modeling and consumer behavior analysis. The repository is structured into two primary modules: **Sales Prediction (SP)** and **Facebook Marketplace (FM)**.

---

## 1. Sales Prediction Analysis
This project evaluates how advertising expenditures across multiple channels—TV, Radio, and Newspapers—influence product sales performance.

### Dataset Overview
* **Observations**: 200 entries recording ad budgets and sales units.
* **Sales Metrics**: Values range from 1.6 to 27 units, with an average of **14.02 units**.
* **Features**: TV, Radio, and Newspaper advertising expenditures.

### Key Analytical Insights
* **TV Dominance**: TV advertising shows the strongest linear relationship with sales (Pearson correlation: **0.78**).
* **Radio Influence**: Radio shows a moderate correlation of **0.58**.
* **Newspaper Inefficiency**: Newspaper impact is negligible (correlation: **0.23**) and is considered an ineffective standalone channel.
* **Predictive Modeling**: Using a linear regression approach, a budget of **TV = $200k, Radio = $40k, Newspaper = $50k** yields a predicted output of **23.53 units**.

---

## 2. Facebook Marketplace Analysis
This module explores engagement patterns of Thai fashion and cosmetics retail sellers on Facebook Live. The analysis aims to optimize content strategy through clustering and engagement trend identification.

### Dataset Overview
* **Source**: UCI Machine Learning Repository.
* **Volume**: 7,050 instances with 14 relevant attributes after preprocessing.
* **Metrics**: Engagement is measured via `num_reactions`, `num_comments`, `num_shares`, and specific reaction types (likes, loves, etc.).

### Core Findings
* **Peak Engagement Time**: Posts shared between **7 PM and 10 PM** attract the highest volume of reactions.
* **Content Strategy**: Video posts generate the highest engagement rates and interactions, followed by photos.
* **Metric Correlations**: Reactions are strongly interlinked with comments (correlation: **~0.78**) and moderately with shares (**~0.62**).
* **Methodology**: K-Means clustering was applied to group sellers, using the **elbow method** to determine the optimal number of clusters.

---

## Repository Structure
The repository is organized as follows:

| Folder | File Name | Description |
| :--- | :--- | :--- |
| **SP** | `Sales_Prediction.ipynb` | Regression modeling and visualization |
| | `advertising_sales_data.xlsx` | Primary dataset for sales analysis |
| | `Sales Prediction Problem Statement.pdf` | Project requirements and objectives |
| **FM** | `Facebook_Marketplace_Analysis.ipynb` | Clustering and engagement analysis |
| | `Facebook_Marketplace_data.csv` | Dataset of Thai retail sellers |
| | `Facebook Marketplace Problem Statement.pdf` | Project requirements and objectives |
| **Results**| `Sales Prediction Analysis.pdf` | Comprehensive report on sales findings |
| | `Facebook Marketplace Analysis.pdf` | Comprehensive report on engagement findings |

---

## Methodology Note
Statistical models used in these projects include:
* **Linear Regression**: Used to predict sales based on multi-channel spend.
* **K-Means Clustering**: Used to segment seller behavior based on engagement metrics.
* **Data Normalization**: Evaluated to determine impacts on model performance.
