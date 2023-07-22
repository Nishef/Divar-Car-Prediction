# Divar-Car-Prediction
## Preprocessing
This code aims to preprocess data extracted from a collection of JSON files.

Joining JSON files into one
The JSON files are stored in a directory, and the first step is to read them all and join them into a single CSV file.

## Data Cleaning
The data cleaning process involves removing columns that are not needed and converting the format of some columns to be more usable. Additionally, some rows with missing values are removed.

## Data Manipulation
The data manipulation process involves converting the values in some columns to a different format, adding missing values, and updating some values based on patterns found in the data.

## Data Visualization
Finally, the data is visualized using a box plot to show the relationship between the year of construction and the lifespan of the cars.

## Libraries Used
pandas
numpy
json
os
pandasgui
plotly.express
## Steps to Run the Code
Install the required libraries using pip install pandas numpy json os pandasgui plotly.express
Download the code and the dataset.
Set the directory containing the JSON files in the json_dir variable.
Run the code. The output of the code will be displayed in the console and in the PandasGui window. The final cleaned dataset will be stored in a CSV file called car1.csv.
