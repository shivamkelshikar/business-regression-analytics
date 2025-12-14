# business-regression-analytics
Interactive business regression analytics tool demonstrating MLE, MAP, and regularized models with real-time visualization and interpretability.
Business Regression Analytics Studio

This project is a web-based interactive tool developed to understand and visualize regression models used in business analytics.
Instead of focusing only on formulas, the project shows how regression models behave when parameters and data change, using real-time graphs and tables.

Student Information
Name: Shivam S. Kelshikar
College: VJTI Mumbai
Course Type: Machine Learning / Data Analytics Project

Purpose of the Project: 
-In many business problems, regression models are used to predict outcomes like sales, revenue, or demand.
-However, most models act like a black box — they give predictions but do not clearly explain why those predictions happen.

The goal of this project is to:
-understand different regression estimation methods
-visualize the effect of regularization
-interpret how each business factor affects the final prediction
-This tool is designed to learn concepts clearly, not just to get numerical output.

Dataset Used:
The dataset used in this project is synthetic but realistic, created to represent a business scenario.

Input Features:
Marketing Spend
Product Price
Customer Footfall
Advertising Spend
Discount Percentage

Output (Target):
-Business Revenue
-The dataset contains 50 samples, with noise added to simulate real business uncertainty.

Regression Methods Implemented: 
1. Ordinary Least Squares (MLE)
-No regularization
-Fits the data by minimizing prediction error
-Sensitive to noise and correlated features

2. Ridge Regression (MAP with L2):
-Adds penalty on large weights
-Produces smoother and more stable models
-Reduces overfitting

3. Lasso Regression (MAP with L1):
-Can reduce some weights to zero
-Helps in feature selection
-Useful when many features are less important

4. Elastic Net:
-Combination of Ridge and Lasso
-Controlled using λ (lambda) and α (alpha)

How the Project Works (Step by Step)
1. Model Selection
The user selects the regression method (OLS, Ridge, Lasso, Elastic Net).
The model updates instantly.

2. Parameter Control:
-λ (lambda) controls the strength of regularization
-α (alpha) controls the balance between L1 and L2 in Elastic Net
-Changing these values updates all results in real time.

3. Prediction and Accuracy Metrics
-The tool calculates and displays:
-Mean Squared Error (MSE)
-Root Mean Squared Error (RMSE)
-R² Score
-L1 and L2 norms
-Sparsity of weights
-These metrics help compare different models.

4. Predicted vs Actual Graph
-This scatter plot compares predicted revenue with actual revenue.
-A straight reference line (y = x) is shown to understand model accuracy visually.

5. Weights Evolution with λ
-This graph shows how each feature’s weight changes as λ increases.
-It clearly explains how regularization shrinks weights and controls model complexity.

6. Feature Sensitivity (What-If Analysis)
-One feature is varied while others are kept constant.
-This helps understand how sensitive the prediction is to changes in a particular business factor.

This is very useful for:
-pricing decisions
-marketing budget planning
-discount analysis

7. Step-by-Step Prediction Breakdown
The tool displays:
-feature value
-learned weight
-contribution (feature × weight)
-This shows exactly how the final prediction is calculated.

8. Correlation Analysis:
-Feature–Feature Correlation (Rxx) shows relationships between input features
-Feature–Target Correlation (Rxy) shows which features influence revenue most
-This helps identify multicollinearity and important variables.

9. Matrices and Dimensions
The project also displays:
-size of feature matrix X
-size of target vector y
-size of weight vector w
-This reinforces the mathematical formulation of regression:
  y=Xw

10. Gaussian Distributions (MLE vs MAP)
The Gaussian plots show:
1.error distribution (likelihood)
2.prior distribution (regularization)
3.posterior distribution (MAP result)
4.This gives an intuitive understanding of why regularization works.
5.How This Project Is Useful for Businesses
6.This project helps businesses to:
7.understand which factors actually drive revenue
8.avoid overfitting while building predictive models

Technologies Used:
1.HTML, CSS, JavaScript
2.Chart.js for visualization
3.GitHub Pages for deployment
4.No backend is required. The project runs completely in the browser.

How to Run the Project:
1.Online
2.Open the GitHub Pages link provided in the repository.
3.Locally
4.Download index.html
5.Open it in any browser
6.No setup required

Conclusion:
This project focuses on understanding regression, not just using it.
By combining mathematical concepts with interactive visualizations, it makes regression models easier to interpret and apply in real business scenarios.
