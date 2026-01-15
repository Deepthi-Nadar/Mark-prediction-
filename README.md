# Linear Regression - Student Mark Prediction

This notebook demonstrates a simple linear regression model to predict student marks based on the number of hours they study.

## Dataset

The dataset used is `Rounded_Student_Hours_Studied_vs_Marks_Dataset.csv`. It contains two columns:

- `Hours_Studied`: The number of hours a student studied.
- `Marks`: The marks obtained by the student.

## Libraries Used

The following Python libraries are used in this notebook:

- `numpy`: For numerical operations.
- `pandas`: For data manipulation and analysis.
- `matplotlib.pyplot`: For data visualization.
- `sklearn.model_selection.train_test_split`: To split data into training and testing sets.
- `sklearn.linear_model.LinearRegression`: To build the linear regression model.
- `sklearn.metrics.r2_score`: To evaluate the model's performance using the R-squared score.

## Steps Involved

1.  **Import Libraries**: Essential libraries like pandas, numpy, and matplotlib are imported.
2.  **Load Dataset**: The dataset `Rounded_Student_Hours_Studied_vs_Marks_Dataset.csv` is loaded into a pandas DataFrame.
3.  **Data Analysis**: Basic descriptive statistics and a scatter plot of 'Hours Studied' vs 'Marks' are generated to understand the data distribution.
4.  **Split Variables**: The dataset is split into independent variable (X - 'Hours_Studied') and dependent variable (y - 'Marks').
5.  **Train/Test Split**: The data is further split into training (80%) and testing (20%) sets to evaluate the model's generalization ability.
6.  **Train Model**: A Simple Linear Regression model is initialized and trained using the training data.
7.  **Predict Results**: Predictions are made on both the training and testing sets.
8.  **Visualize Results**: Scatter plots are generated to visualize the regression line on both the training and test sets.
9.  **Model Evaluation**: The coefficient (slope), intercept, and R-squared score are calculated to assess the model's accuracy.
10. **Predict New Values**: The trained model is used to predict marks for a new input of study hours.


## Results

-   **Coefficient (Slope)**: The model determined a coefficient (slope) of approximately `5.25`. This means for every additional hour studied, the marks are predicted to increase by `5.25`.
-   **Intercept**: The model's intercept is approximately `18.09`. This represents the predicted marks when the hours studied are zero.
-   **R-squared Score**: The model achieved an R-squared score of approximately `89.25%` on the test set, indicating that about `89.25%` of the variance in marks can be explained by the hours studied.
-   **Prediction Example**: For a student studying `7` hours, the predicted marks are approximately `54.83`.

