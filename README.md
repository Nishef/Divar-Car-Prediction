# Divar-Car-Prediction(Tehran)
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
-pandas
-numpy
-json
-os
-pandasgui
-plotly.express
## Steps to Run the Code
Install the required libraries using pip install pandas numpy json os pandasgui plotly.express
Download the code and the dataset.
Set the directory containing the JSON files in the json_dir variable.
Run the code. The output of the code will be displayed in the console and in the PandasGui window. The final cleaned dataset will be stored in a CSV file called car1.csv.
## Data Preprocessing Steps
-Joining all 45527 JSON files into one JSON file
-Reading the CSV file created from the JSON data
-Selecting the relevant columns
-Handling missing values
-Converting Persian numbers to English numbers
-Extracting numerical values from string columns
-Removing non-numeric characters from the 'Price' column
-Replacing NaN values with a default value
-Converting the 'Price' column to integer data type
-Converting the 'YearOfConstruction' column to the Jalali calendar
-Identifying and extracting fuel type and gearbox information from the 'Brand' column
-Filtering out rows with 'YearOfConstruction' values less than or equal to 1390 and 'LifeSpan' values equal to 0
-Filtering out rows with 'YearOfConstruction' less than or equal to 1373 and 'LifeSpan' less than 100000
-Removing rows where the 'Price' column is less than 45e6
-Filtering out rows where 'Price' is less than or equal to 1e8 and 'YearOfConstruction' is greater than or equal to 1390
-Replacing incorrect values in the 'Price' column for the 'پورشه ماکان' brand.
-Handling missing values by filling them with the mode of each column.
-The final output of the code is a cleaned and processed CSV file.
### to-do:
- [x] Preprocessing
- [x] Visualizing
- [ ] Machine-Learning
- [ ] Maybe some deep-learning

