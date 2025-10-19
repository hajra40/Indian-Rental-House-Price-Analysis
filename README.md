# Indian-Rental-House-Price-Analysis

## About the Data
This project analyzes rental house prices across various cities in India using a dataset scraped from Makaan.com in April 2024. The dataset includes detailed information such as house type, size, location, price, number of bathrooms and balconies, furnishing status, and more.

Link: https://www.kaggle.com/datasets/bhavyadhingra00020/india-rental-house-price

## Data Processing Using Python

The dataset underwent a complete data cleaning and transformation process to prepare it for advanced rental market analysis in Power BI. Starting with 13,910 raw records collected from multiple Indian cities, the data was standardized, merged, and expanded to a unified dataset of 13,910 entries. Missing values in numerical fields such as bathrooms, balconies, and negotiability were replaced with zeros, while text fields were cleaned and normalized. Key engineered features included extracting numeric values from house size (house_size_num) and computing rental efficiency through rentPerSqft (price per square foot). Additional processing ensured consistent data types, accurate geographic coordinates, and removal of empty or redundant columns. The final dataset—containing 18 well-structured columns—provides a comprehensive, analysis-ready view of the Indian rental housing market, enabling geospatial, trend-based, and comparative insights into rental pricing and property characteristics.

### Cleaned Data
<img width="1799" height="746" alt="image" src="https://github.com/user-attachments/assets/d3de1313-7370-425d-a453-c54c31d84e5b" />
<img width="457" height="473" alt="image" src="https://github.com/user-attachments/assets/055833c7-4ce7-48fa-818d-c5327dd23b08" />

## Power BI Dashboard

### Page 1 - Rental Overview Dashboard

This Power BI dashboard provides an interactive overview of rental housing trends across major Indian cities, including Mumbai, Hisar, Delhi, and Pune. It highlights key rental metrics such as average price, rent per square foot, number of bedrooms (BHK), bathrooms, and security deposits. Users can filter by city, property type, and price range to explore detailed insights. The KPI cards present quick summaries of major indicators — with an average rent of ₹44.71K and rent-per-sq.ft of ₹40.76 across the dataset.

Visual analyses show that Mumbai commands the highest average rents (₹62.4K) and rental intensity, while Pune offers more affordable options at around ₹22K. A decomposition of furnishing status reveals that furnished and semi-furnished properties consistently attract higher rents compared to unfurnished units. The negotiability distribution chart indicates that rental flexibility varies across cities and furnishing types.

Overall, the dashboard enables users to compare city-wise rental patterns, assess how furnishing and amenities affect rent, and identify the most expensive and negotiable markets within India’s April 2024 rental landscape.

<img width="1376" height="699" alt="image" src="https://github.com/user-attachments/assets/a1c13cf9-81a2-472b-b4e2-39abe631b55d" />

### Page 2 - Geographic Overview of Rental Prices Across Major Locations
<img width="1527" height="859" alt="image" src="https://github.com/user-attachments/assets/a491c464-4c7b-4528-bca2-f93dce826277" />

### Page 3,4 & 5 - Decomposition Tree & Key Influencers

<img width="1530" height="853" alt="image" src="https://github.com/user-attachments/assets/9efe5d56-3bb4-43a2-81cc-f8dc9e3bfc53" />
<img width="1515" height="821" alt="image" src="https://github.com/user-attachments/assets/5439de44-9461-427d-8edf-f35875169978" />
<img width="1579" height="791" alt="image" src="https://github.com/user-attachments/assets/58cf2177-c35c-4759-87a8-c4bcfb7d905d" />
<img width="1700" height="750" alt="image" src="https://github.com/user-attachments/assets/220c0c18-cfca-4d30-90ab-2504b14f2d37" />




