# 🍷 Wine Quality Linear Regression Analysis

This project analyzes the factors influencing wine quality using a linear regression model. The dataset includes various physicochemical properties of wine, and the goal is to identify which variables significantly predict wine quality.

## 📊 Objective

- Build and evaluate a multiple linear regression model to predict wine quality.
- Identify statistically significant predictors.
- Validate model assumptions.
- Visualize relationships between predictors and wine quality.

##  📁 Dataset
- The dataset used contains 788 wine samples with the following features:
- fixed acidity
- volatile acidity
- citric acid
- residual sugar
- chlorides
- free sulfur dioxide
- total sulfur dioxide
- density
- pH
- sulphates
- alcohol
- quality (target)

## 🧪 Methodology

### 🧠 Refined Model and key Insight
A full linear regression was honed through two iterations to only include significant predictors and maximize the accuracy and explanatory power of coefficients. RobustScaling was used.

R² = 0.341, Adjusted R² = 0.338.
Model summary showed only 3 features were statistically significant (p < 0.05):
volatile acidity (p < 0.001, β = -0.2733)
chloridess (p < 0.001, β = -0.0391)
total sulfur dioxide (p < 0.001, β = -0.1045)
sulphates (p < 0.001, β = 0.1669)
alcohol (p < 0.001, β = 0.4289)

### ✅ Assumptions Checked
Linearity: Mostly confirmed via residuals vs. fitted values plot.

Independence of Errors: Supported by a Durbin-Watson statistic close to 2.

Homoscedasticity: Residuals plot showed no clear funneling pattern.

Normality of Errors: Q-Q plot of residuals closely followed the normal line.

Mean of Errors ≈ 0: Mean error ≈ 1.57e-13.

High-leverage Points: Identified using Cook’s Distance; though no points were removed.

Multicollinearity: Checked using VIF; all variables in final model had VIF < 5.

## Improvements for Future Analysis
- Splitting the data into testing and training data before scaling it, as otherwise the testing data is no longer truly independent
- The heatmap I used for correlations could have had a fuller scale (i.e., -1 to 1) to help contextualize differences



