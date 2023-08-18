# Divar-Car-Prediction(Tehran)
The presented code is based on real car data collected from the [Divar website](https://divar.ir/s/tehran/vehicles) until the spring of 1402. The data was consolidated into a comprehensive file, which was then subjected to various techniques to improve its quality and reduce noise and errors. These techniques aimed to make the data more suitable for further analysis and learning purposes. The resulting dataset and the techniques used to improve it are available for use and can be accessed for further study.
## Installation
To run this code, you need to have the following dependencies installed:

- matplotlib
- numpy
- pandas
- seaborn
- pandasgui(optional)
- scikit-learn
  
You can install these dependencies using pip:
```
pip install matplotlib numpy pandas seaborn pandasgui scikit-learn
```
## Usage
Clone the repository or download the code files.
Make sure you have the required dependencies installed.
Run the code using a Python IDE or Jupyter Notebook.
Data
The data used in this project is stored in a CSV file named car_final.csv. It contains information about various cars, including their features and prices.

## Exploratory Data Analysis
The code begins with an exploratory data analysis to gain insights into the dataset. It includes checking for null values, displaying DataFrame information, and creating a correlation matrix heatmap to visualize the relationships between different features.

## Data Preprocessing
Before training the models, the data is preprocessed to transform categorical variables into numerical representations using label encoding. The dataset is then split into training and testing sets.

## Random Forest Regression
A Random Forest regressor is trained using the training data. The code specifies the number of estimators and maximum depth for the Random Forest model.

## Model Evaluation
The performance of the trained model is evaluated using various metrics, including R-squared, mean squared error (MSE), and mean absolute error (MAE). The code calculates these metrics and prints the results.

## Residual Analysis
Residual analysis is performed to examine the distribution of residuals, which represent the differences between the predicted and actual car prices. The code generates histograms and density plots to visualize the distribution of residuals and identify potential outliers.

## Outlier Removal
Outliers with extremely high residual values are removed from the dataset. The code filters out rows where the absolute difference between the actual and predicted prices exceeds a threshold.

## Feature Importance Analysis
The importance of each feature in predicting car prices is analyzed using the trained Random Forest model. The code calculates feature importances and visualizes them in a bar plot. The plot provides insights into the relative importance of different features in determining the car prices.

## Result
Before removing outliers and cleaning the data, the model achieved the following results:

- R-squared: 0.891
- MSE: 134,155,034,425,309,360.00
- MAE: 111,245,727.10

After training and evaluating the Random Forest regression model, the following results were obtained:

- R-squared: 0.970
- MSE: 11,411,474,984,066,076.00
- MAE: 33,759,678.07

## Conclusion
The results indicate a significant improvement in the model's performance after removing outliers and cleaning the data. The R-squared value of 0.970 suggests that the model can explain 97% of the variance in the car prices. The lower MSE and MAE values (11,411,474,984,066,076.00 and 33,759,678.07, respectively) indicate smaller errors between the predicted and actual car prices.

The initial model, without data cleaning, had a lower R-squared value of 0.891 and higher MSE and MAE values (134,155,034,425,309,360.00 and 111,245,727.10, respectively). This indicates that the model's performance was significantly improved by removing outliers and cleaning the data.

Based on these results, we can conclude that the Random Forest regression model, trained on the cleaned dataset, is effective in predicting car prices. It captures important relationships between the features and target variable, leading to accurate price predictions. Further improvements could be made by exploring other regression algorithms, feature engineering techniques, or fine-tuning the model's hyperparameters.

Feel free to modify the code and experiment with different parameters to further improve the performance or explore additional aspects of the data.
### to-do:
- [x] Preprocessing
- [x] Visualizing
- [x] Machine-Learning
- [ ] Maybe some deep-learning

