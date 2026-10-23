Sales Prediction Model Using Machine Learning

1. Project Overview

This project focuses on predicting product sales using historical sales data and machine learning techniques. The main objective is to build and evaluate regression models that can estimate sales based on selected product and transaction features.

The project uses the Sample Superstore dataset and compares Linear Regression and Random Forest Regression to understand how different machine learning models perform on the same dataset.

2. Objectives

- Analyze historical sales data.
- Identify useful features for sales prediction.
- Prepare the dataset for machine learning.
- Train regression models using the prepared data.
- Evaluate model performance using standard regression metrics.
- Visualize actual sales compared with predicted sales.
- Identify limitations and possible improvements.

3. Dataset Description

The Sample Superstore dataset contains sales transaction records with information about products, categories, regions, quantities, discounts, and sales.

The features selected for this project include:

- Quantity: Number of items in a transaction.
- Discount: Discount applied to the transaction.
- Category: General product category.
- Sub-Category: Specific product group.
- Region: Geographic sales region.

Target variable: Sales — the numerical value the models are trained to predict.

4. Tools and Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Google Colab
- GitHub

5. Project Workflow

Step 1: Data Loading

The dataset is loaded into a Pandas DataFrame for analysis and preparation.

Step 2: Feature Selection

Relevant columns are selected as input features, while Sales is selected as the target variable.

Step 3: Data Encoding

Categorical variables such as Category, Sub-Category, and Region are converted into numerical columns using one-hot encoding.

Step 4: Train-Test Split

The dataset is divided into training and testing sets. The training set is used to fit the models, while the testing set is used to evaluate their performance on unseen records.

Step 5: Model Training

Two regression models are trained:

- Linear Regression: A basic regression model used as a starting point for sales prediction.
- Random Forest Regression: An ensemble model that combines multiple decision trees to capture more complex relationships in the data.

Step 6: Model Evaluation

The models are evaluated using the following metrics:

- MAE (Mean Absolute Error): Measures the average absolute difference between actual and predicted sales.
- RMSE (Root Mean Squared Error): Measures prediction error while penalizing larger errors more heavily.
- R² Score: Indicates how much variation in the target variable is explained by the model.

Step 7: Visualization

Actual versus predicted sales graphs are created using Matplotlib to visually inspect prediction performance and identify errors, particularly for high-sales transactions.

6. Key Results

Based on the recorded evaluation results, the Random Forest model achieved:

- MAE: Approximately 200.71
- RMSE: Approximately 674.61
- R² Score: Approximately 0.2296

The Random Forest model performed better than Linear Regression across the three evaluation metrics in this experiment.

The R² score indicates that the model explains approximately 22.96% of the variation in sales. The actual-versus-predicted plot also shows that predictions for some high-sales transactions are substantially lower than their actual values.

7. Key Insights

- Random Forest Regression performed better than the Linear Regression baseline on the test data.
- Prediction errors were generally smaller for many low- and moderate-sales records than for some high-sales records.
- Some high-value transactions were underestimated.
- The current features provide useful information but do not explain all the variation in sales.
- Additional relevant features and improved model tuning may help improve prediction performance.

8. Limitations and Future Improvements

The model has limitations, including prediction errors for high-sales transactions and a relatively low R² score.

Possible improvements include:

- Adding more relevant features.
- Investigating outliers and unusual transactions.
- Performing hyperparameter tuning.
- Comparing additional regression algorithms.
- Using a dataset with suitable date information if time-based sales forecasting is required.

9. Conclusion

This project demonstrates a complete introductory machine learning workflow for sales prediction, from data preparation and feature encoding to model training, evaluation, and visualization.

By comparing Linear Regression and Random Forest Regression, the project shows how different models can produce different prediction results. Although the Random Forest model performed better in this experiment, further improvements are needed to predict high-sales transactions more accurately.

10. Project Files

- "project2_model.ipynb" — Complete notebook containing the code, model training, evaluation results, and visualizations.
- "README.md" — Project overview, workflow, results, and conclusion.

11. How to Run

1. Open the notebook in Google Colab.
2. Upload the required Sample Superstore CSV dataset.
3. Run the notebook cells in order.
4. Review the model evaluation metrics and visualizations.

---

Project Type: Machine Learning — Regression
Status: Completed
Environment: Google Colab
Repository: "sales-prediction-model"
