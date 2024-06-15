# Zomato Restaurant Analysis

## Project Overview

This project involves the analysis of restaurant data from Zomato to gain insights into various aspects such as average cost, ratings, and cuisines offered by restaurants in the United States. The dataset used for this analysis consists of information about restaurants from various cities around the world.

## Dataset Description

The analysis is performed on two files:
1. **zomato.csv**: Contains detailed information about restaurants.
2. **country-code.xlsx**: Contains country codes and corresponding country names.

The two files are merged using the country code, and the analysis is focused on restaurants located in the United States.

### Attributes in the Dataset

- **Restaurant Id**: Unique id of every restaurant across various cities of the world.
- **Restaurant Name**: Name of the restaurant.
- **Country Code**: Country in which the restaurant is located.
- **City**: City in which the restaurant is located.
- **Address**: Address of the restaurant.
- **Locality**: Location in the city.
- **Locality Verbose**: Detailed description of the locality.
- **Longitude**: Longitude coordinate of the restaurant's location.
- **Latitude**: Latitude coordinate of the restaurant's location.
- **Cuisines**: Cuisines offered by the restaurant.
- **Average Cost for two**: Cost for two people in different currencies.
- **Currency**: Currency of the country.
- **Has Table booking**: Indicates if the restaurant has table booking (yes/no).
- **Has Online delivery**: Indicates if the restaurant has online delivery (yes/no).
- **Is delivering**: Indicates if the restaurant is currently delivering (yes/no).
- **Switch to order menu**: Indicates if the restaurant has switched to an order menu (yes/no).
- **Price range**: Range of price of food.
- **Aggregate Rating**: Average rating out of 5.
- **Rating color**: Color code depending upon the average rating.
- **Rating text**: Text description based on the rating.
- **Votes**: Number of ratings cast by people.

## Data Processing and Analysis

### Data Filtering
- The data is filtered to include only the restaurants located in the United States.

### Data Transformation
- Categorical textual inputs for 'Has Table booking', 'Has Online delivery', and 'Switch to order menu' are converted from yes/no to 1/0 for analysis.

### Visualization
- Bar charts and histograms for Rating text were plotted to get a clear idea of the distribution of ratings.
- A geographical map was plotted to visualize the distribution of aggregate ratings across different locations.

### Model Building
- The data was scaled using MinMaxScaler to normalize the values.
- The dataset was split into training and testing sets using train-test split.
- A Linear Regression model was fitted on the data to predict the average cost for two people.
- A Decision Tree Regression model was also used to compare the results with the Linear Regression model.

### Cuisines Analysis
- The cuisines served in all restaurants were analyzed to understand the variety and popularity of different cuisines.

## Results
- The analysis provided insights into the average cost for two people in US restaurants.
- The geographical distribution of ratings helped identify areas with highly-rated restaurants.
- The performance of the Linear Regression model and Decision Tree Regression model in predicting the average cost was compared.

## Conclusion
This project provides a comprehensive analysis of restaurant data in the United States, offering insights into costs, ratings, and cuisines. The models used can help predict costs and understand various factors affecting restaurant ratings and popularity.

## How to Run the Project

1. Ensure you have the necessary libraries installed:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```

2. Load the datasets and merge them on the country code.

3. Filter the data to include only US restaurants.

4. Perform the necessary data transformations and visualizations.

5. Scale the data and split it into training and testing sets.

6. Fit the Linear Regression and Decision Tree Regression models.

7. Analyze the results and compare the model performances.
