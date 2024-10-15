# Spaceship Titanic

### Introduction

In Kaggle's competition, the task is to predict whether a passenger was transported to an alternate dimension during the Spaceship Titanic's collision with a spacetime anomaly. 

To assist with these predictions, a set of personal records, recovered from the ship's damaged computer system, is provided.

### Goal

The goal of this project is to develop a model that identifies passengers who were transported to an alternate dimension.

### Objectives

To achieve this goal, the following objectives have been established:

- Download, load and clean the dataset.
- Conduct exploratory data analysis and visualize data to identify underlying patterns.
- Perform statistical inference to validate findings.
- Apply machine learning models to predict which passengers were lost.
- Summarize results and provide actionable recommendations based on the analysis.

## Exploratory Data Analysis

In this section, the dataset is explored by performing the following:

- Uploading and providing an overview of the dataset
- Generating charts and summaries to visualize key insights
- Analyzing statistics to identify correlations between features and the target variable

## Feature Engineering 

Before training machine learning models, the dataset is prepared by:

- Generating new features to uncover valuable patterns
- Reducing missing data by establishing rules based on passenger relationships and filling values logically
- 
## Statistical Inference

This section focuses on statistical inference to evaluate:

- Whether there is a difference in the distribution of age between individuals who were transported and those who were not.
- The significance of the correlation between categorical independent variables and the dependent variable.

## Statistical Modeling

In this section, statistical modeling is performed by:

- Training and evaluating multiple classifiers, including LGBM, XGBoost, and CatBoost
- Conducting hyperparameter tuning using Random Search
- Combining the three best models into a stacking classifier

## Conclusions

Here’s a concise summary of your exploratory data analysis, statistical inference, and modeling sections:

- **Exploratory Data Analysis**: The target variable "Transported" is nearly balanced, with key features like CryoSleep and HomePlanet significantly influencing transportation rates. Insights reveal younger passengers are transported more frequently, while higher service expenditures decrease the likelihood of transportation.

- **Missing Values**: Identified that 24% of rows had missing entries; updated the dataset accordingly and established rules for further imputation.

- **Statistical Inference**: A significant difference in age distributions was found between transported and non-transported passengers. Significant associations were also observed between categorical variables, with p-values below the adjusted significance level.

- **Model Performance**: Among LGBM, CatBoost, and XGBoost, CatBoost exhibited the highest validation accuracy. The stacking classifier combining these models slightly outperformed individual models.

- **Evaluation Metrics**: The stacking classifier showed balanced performance in precision, recall, and F1-score, with an AUC of 0.88 confirming strong predictive capabilities.

- **Feature Importance**: Service Expenditure emerged as the most influential feature in predictions, followed by other expenditure features, Home Planet, and Cabin Decks, while Age Groups and Traveling Solo had lesser importance. SHAP analysis corroborated these findings.

## License

This project is licensed under the [MIT License](LICENSE).

