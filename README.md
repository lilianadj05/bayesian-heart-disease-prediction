# ❤️‍🩹 Heart Disease Bayesian Data Analysis

## 📌 Project Overview
This project uses Bayesian methods to analyze a heart disease dataset, comparing two logistic regression models: one with uninformative priors and another with informative priors. The goal is to determine which model better predicts heart disease presence and to interpret the results to identify significant predictors.

## 📊 Dataset
The project uses the **Heart Disease Dataset** from the UCI Machine Learning Repository. It contains 303 observations and 14 variables, including demographic information, medical test results, and a target variable indicating the presence of heart disease.

## 🔍 Key Findings
1. **Model Comparison**: The model using informative priors (Model 2) demonstrates a better fit and predictive performance compared to the model with uninformative priors (Model 1), as indicated by a lower WAIC score and Bayes factor.
2. **Significant Predictors**: The analysis reveals that age, sex, chest pain type, resting blood pressure, cholesterol, resting electrocardiographic results, exercise-induced angina, the slope of the peak exercise ST segment, and thalassemia are all significant predictors of heart disease.
3. **Posterior Predictive Check**: The final model shows a notable misfit when compared to the observed data, suggesting that the model's predictions for the proportion of patients with heart disease do not align well with the actual data. This indicates the model may be misspecified or is missing important variables.

## 📈 Steps
1. **Data Preprocessing**: The dataset was read into the R environment, and the predictor variables were scaled. The target variable and scaled predictors were then prepared for modeling.
2. **Model Building**: Two Bayesian logistic regression models were built using JAGS: Model 1 with uninformative priors (normal distribution with mean 0 and precision 0.01) and Model 2 with informative priors based on published journal findings.
3. **Model Evaluation**: The models were evaluated using convergence diagnostics, including trace plots, autocorrelation, effective sample size (ESS), Gelman-Rubin diagnostics, and Geweke diagnostics. The models were also compared using the Bayes factor, WAIC, and posterior predictive checks.
4. **Interpretation**: The best-performing model (Model 2) was interpreted by examining the 95% credible intervals of its coefficients to identify significant predictors of heart disease.

## 💡 Conclusion
The Bayesian **logistic regression model with informative priors** was found to be the better of the two models for predicting heart disease. The analysis identified several key predictors, providing insight into the factors associated with heart disease. However, the posterior predictive checks revealed a significant limitation, indicating that the model's predictive capabilities are not fully aligned with the observed data.

## 🔮 Possible Future Work
1. **Feature Engineering**: Explore creating new variables or interaction terms to improve the model's fit.
2. **Advanced Models**: Investigate more complex models or different prior distributions to address the observed misfit.
3. **Data Collection**: Consider a larger or more diverse dataset to enhance the model's generalizability and predictive accuracy.

## 🤝 Contributors
1. Leony Sani Winata
2. Liliana Djaja Witama
3. Angeli Jessica Wibowo
4. Felicia Audrey Tanujaya
