# Bangalore-House-Price-Prediction

  Machine learning project to predict Bangalore house prices using Linear Regression, with 85% accuracy after data cleaning, feature engineering, and outlier removal
  
📌 Project Overview

  This project focuses on predicting house prices in Bangalore using machine learning techniques. The analysis involves data cleaning, feature engineering, and building a predictive model to estimate property prices based on various features such as location, square footage, number of bedrooms, and bathrooms.

📊 Dataset Details

The dataset used in this project is Bengaluru_House_Data.csv, which contains 13,320 entries with the following features:

• area_type: Type of area (e.g., Super built-up, Plot, Built-up)

• availability: Availability status of the property

• location: Neighborhood location

• size: Number of bedrooms (e.g., 2 BHK, 3 BHK)

• society: Housing society name

• total_sqft: Total square footage

• bath: Number of bathrooms

• balcony: Number of balconies

• price: Price of the property (in lakhs)

⦾ Steps Performed

1. Data Cleaning

• Removed unnecessary columns (area_type, society, balcony, availability).

• Handled missing values by dropping rows with null entries.

• Extracted the number of bedrooms (bhk) from the size column.

• Cleaned the total_sqft column by converting ranges (e.g., "1000-1500") to average values.

2. Feature Engineering

• Created a new feature price_per_sqft to analyze the relationship between price and square footage.

• Grouped less frequent locations under the "other" category to reduce dimensionality.

3. Outlier Detection and Removal

• Removed properties where the square footage per bedroom was less than 300 sq ft.

• Applied statistical methods to remove outliers in the price_per_sqft feature based on standard deviation.

4. Data Visualization

• Used scatter plots to visualize the relationship between square footage and price for different bedroom configurations (e.g., 2 BHK vs. 3 BHK).

⦾ Key Insights

• The dataset initially contained 13,320 entries, which was reduced to 10,222 after cleaning and outlier removal.

• Properties with unusually low square footage per bedroom were identified and removed.

• The price_per_sqft feature was normalized to reduce the impact of extreme values.

⦾ Tools and Libraries

• Python: Primary programming language

• Pandas: Data manipulation and analysis

• NumPy: Numerical computations

• Matplotlib & Seaborn: Data visualization

🔮 Next Steps

• Implement machine learning models for price prediction

• Perform model tuning and validation

• Develop web application for real-time predictions

• Expand analysis to other Indian cities
