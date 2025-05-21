# Housing Price Prediction - King County Real Estate

## Project Overview
This project analyzes residential real estate data from King County, which includes Seattle. The goal is to predict house prices based on various features such as square footage, number of bedrooms, number of floors, waterfront view, and more. The analysis involves data cleaning, exploratory data analysis (EDA), and building regression models to estimate market prices of houses.

## Dataset
The dataset contains house sales between May 2014 and May 2015 and includes the following features:

- `price`: Sale price of the house (target variable)
- `bedrooms`: Number of bedrooms
- `bathrooms`: Number of bathrooms
- `sqft_living`: Square footage of the living area
- `sqft_lot`: Square footage of the lot
- `floors`: Number of floors in the house
- `waterfront`: Whether the house has a waterfront view (0 = No, 1 = Yes)
- `view`: Quality of the view from the house
- `condition`: Overall condition rating
- `grade`: Overall grade based on King County grading system
- `sqft_above`: Square footage excluding basement
- `sqft_basement`: Square footage of the basement
- `yr_built`: Year the house was built
- `yr_renovated`: Year the house was renovated
- `zipcode`: Zip code location
- `lat`, `long`: Latitude and longitude coordinates
- `sqft_living15`: Living room area in 2015 (post-renovation)
- `sqft_lot15`: Lot size in 2015 (post-renovation)

## Steps Performed
1. **Data Import & Cleaning**: Loaded the dataset, dropped irrelevant columns (`id`, `Unnamed: 0`), and handled missing values by replacing NaNs with column means.
2. **Exploratory Data Analysis (EDA)**:
   - Analyzed distribution of floors.
   - Visualized price outliers with respect to waterfront view using boxplots.
   - Investigated relationships between features like `sqft_above` and price using regression plots.
3. **Correlation Analysis**: Identified which features correlate most strongly with house price.
4. **Model Development**:
   - Built simple linear regression models to predict price using features like `long` and `sqft_living`.
   - Evaluated model performance using R² scores.
5. **Further Analysis**: Additional models and feature engineering planned to improve price prediction accuracy.

## Libraries Used
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## How to Run
1. Download the dataset or load it directly from the provided URL.
2. Run the Jupyter Notebook cells sequentially to reproduce the analysis and modeling steps.
3. Review the outputs, charts, and regression results for insights.

