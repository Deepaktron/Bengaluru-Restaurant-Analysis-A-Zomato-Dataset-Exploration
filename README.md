# Bengaluru Restaurant Analysis: A Zomato Dataset Exploration

## Project Description: Bengaluru Restaurant Analysis

### Project Overview

The objective of this project is to conduct a comprehensive analysis of restaurants in Bengaluru using data from Zomato. This analysis focuses on various aspects including restaurant ratings, types, locations, cuisines, and customer engagement metrics. The insights derived from this analysis will help in understanding the dining landscape of Bengaluru, identifying popular areas and cuisines, and uncovering patterns in customer preferences and behavior.

### Data Description

The dataset comprises various features capturing different aspects of Bengaluru restaurants:

- **URL**: Unique URL of the restaurant's Zomato page.
- **Name**: The name of the restaurant.
- **Phone**: Contact numbers of the restaurant.
- **Location**: Geographical location of the restaurant within Bengaluru.
- **Resting**: The type of establishment (e.g., Casual Dining, Cafe).
- **Cuisines**: Types of cuisines offered by the restaurant.
- **Dish Liked**: Popular dishes liked by customers.
- **Ratings**: Average rating of the restaurant.
- **Votes**: Number of votes the restaurant has received.
- **Online Order**: Indicates whether the restaurant accepts online orders.
- **Book Table**: Indicates whether table booking is available.
- **Approx Cost**: Approximate cost for two people.
- **Type**: The category of the restaurant (e.g., Delivery, Dine-out).
- **City**: The city where the restaurant is located.

### Data Cleaning Process

#### Initial Data Exploration
- **Library Imports**: Pandas for data manipulation and NumPy for numerical operations.
- **Data Loading**: Loaded the dataset using `pd.read_csv`.
- **Inspection**: Inspected the first 20 rows and checked the dataset information and null values count.

#### Data Cleaning - Phase 1
- **Column Renaming**: Renamed columns for clarity and consistency.
- **Duplicate Removal**: Removed duplicate entries in 'name', 'address', and 'phone' columns.
- **Text Normalization**: Cleaned 'name' column for any unusual or encoded entries.
- **Phone Number Formatting**: Standardized phone numbers by replacing inconsistent delimiters.
- **Ratings Cleaning**: Converted rating entries to numerical values and removed non-numerical values.
- **Votes Conversion**: Converted 'votes' column to numeric values.
- **Categorical Columns Cleaning**: Standardized values in 'online order' and 'book table' columns.
- **Alphabetic Filtering**: Removed non-alphabetic values from 'location', 'resting', 'cuisines', 'dish liked', and 'city' columns.
- **Menu and Reviews Cleaning**: Cleaned 'menu' and 'reviews' columns by removing unnecessary characters.

#### Data Cleaning - Phase 2
- **Null Values Handling**: Removed rows with null values in critical columns such as 'name', 'ratings', 'phone', 'cuisines', 'dish liked', 'resting', 'location', and 'approx cost'.
- **Final Export**: Exported the cleaned dataset for further analysis.

### Analysis Breakdown

#### 1. Restaurant Ratings Analysis
- **Rating Distribution**: Analyze the distribution of restaurant ratings to understand the quality of restaurants in Bengaluru.
- **Top Rated Restaurants**: Identify the top-rated restaurants and explore their characteristics.

#### 2. Cuisine Analysis
- **Popular Cuisines**: Determine the most popular cuisines offered by restaurants in Bengaluru.
- **Cuisine and Rating Correlation**: Analyze the correlation between different cuisines and their ratings.

#### 3. Geographic Analysis
- **Location Insights**: Explore the distribution of restaurants across different locations in Bengaluru.
- **Popular Areas**: Identify areas with the highest concentration of restaurants and high-rated establishments.

#### 4. Cost Analysis
- **Cost Distribution**: Analyze the distribution of approximate costs for dining to understand the pricing landscape.
- **Cost and Rating Relationship**: Investigate the relationship between cost and restaurant ratings.

#### 5. Customer Engagement
- **Online Orders and Bookings**: Examine the prevalence of online ordering and table booking options.
- **Customer Feedback**: Analyze customer reviews and ratings to gain insights into customer satisfaction and preferences.

### Tools and Libraries Used

- **Pandas**: For efficient data manipulation, cleaning, and analysis.
- **NumPy**: For numerical computations and array operations.
- **Matplotlib**: For creating static, interactive, and animated visualizations in Python.
- **Seaborn**: For statistical data visualization, based on Matplotlib.
- **unicodedata**: For text normalization and cleaning.

### Conclusion

This comprehensive analysis of Bengaluru restaurants using the Zomato dataset provides valuable insights into the dining trends and customer preferences in the city. By understanding these patterns, restaurant owners and marketers can optimize their offerings, enhance customer experiences, and develop targeted strategies to attract and retain customers. The results of this analysis will help in better serving the diverse culinary preferences of Bengaluru's residents and visitors, ultimately contributing to the growth and success of the restaurant industry in the city.
