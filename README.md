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


## Key Insights

1. City-wise Rental Market Landscape
Delhi is the most expensive place in terms of property's monthly rent and cost per unit of area. It has an average rent price of 222.17K and highest average rental price intensity at 59.34 per sq. ft. At second place is Mumbai but it has an average price less than that of Delhi by about 71%.
General hierarchy for avg rent is: Delhi > Mumbai > Pune > Hisar.
While Pune's average rent (approx. ₹29.19K) is higher than Hisar's, Hisar has a significantly higher average rental price per square foot (₹54.57) compared to Pune (₹21.91). This suggests that rental properties in Hisar are, on average, smaller than in Pune but command a higher price for the space they offer.

3. Influence of Furnishing Status
Furnished Properties Command Higher Rents: As stated on the treemap, furnished and semi-furnished properties have higher average rents than unfurnished ones across most cities. For example, in Mumbai, the average rent for a semi-furnished property is ₹65.81K, and for a furnished one, it is ₹87.59K.
Major Outlier in Delhi: The data for unfurnished properties in Delhi shows an average rent of ₹395.12K. This is a massive outlier, being almost double the average rent of the most expensive city (Mumbai). This could be due to:
- A data entry error.
- The inclusion of a few ultra-luxury commercial or residential properties that are skewing the average.
- A very small sample size for this specific category. This data point requires immediate investigation to verify its accuracy.

3. Property Characteristics and Pricing
Positive Correlation: The dashboard notes that the average price is positively correlated with the average number of BHKs (Bedrooms, Hall, Kitchen) and bathrooms. The "City-wise Comparison" chart visually supports this, showing that Mumbai, the city with the highest average price, also has the highest average number of BHKs (1.87) and bathrooms (2.03).

4. Market Negotiability
<img width="1530" height="853" alt="image" src="https://github.com/user-attachments/assets/9efe5d56-3bb4-43a2-81cc-f8dc9e3bfc53" />
<img width="1515" height="821" alt="image" src="https://github.com/user-attachments/assets/5439de44-9461-427d-8edf-f35875169978" />
<img width="1579" height="791" alt="image" src="https://github.com/user-attachments/assets/58cf2177-c35c-4759-87a8-c4bcfb7d905d" />
Out of all the data, only 9% of the houses are negotiable for the rental prices and with average price of around 1.14 lakhs - with Delhi being at the top for most non-negotiable rental house prices followed by Mumbai & Pune. Among the 9% negotiable properties, Mumbai & Pune covers 85.5% of the houses with an average price of ~80K & ~26K. 
Hisar having the lowest count of houses for both negotiable and non-negotiable, it still has the highest rental of around ~94K.
Negotiability Rate Hierarchy: Hisar (38%) > Pune (13%) > Mumbai (11%) > Delhi (4%)

4. Key Influencers
<img width="1700" height="750" alt="image" src="https://github.com/user-attachments/assets/220c0c18-cfca-4d30-90ab-2504b14f2d37" />
1. The type of property is the most significant factor influencing the size of the security deposit. The analysis highlights that luxury or standalone properties command substantially higher deposits than standard apartments or floors. When the property is a Villa, the average security deposit increases by a massive ₹1.6 million. This is the single most powerful influencer identified. Similarly, an Independent House also has a major impact, increasing the average deposit by ₹1.04 million. An Independent Floor increases the deposit by a more moderate ₹333,900.
The bar chart on the right provides a clear visual confirmation of this hierarchy. Penthouses demand the absolute highest average security deposit (approximately ₹3.5M), followed closely by Villas (the selected influencer, at approx. ₹1.8M). Both are dramatically higher than the deposits for Independent Floors or Apartments.

2. While property type is dominant, other factors also play a key role in increasing the security deposit amount. City: Being located in Delhi increases the average security deposit by ₹597,800. This suggests that landlords in Delhi, likely due to higher rental values and perceived risks, demand significantly higher upfront security than in other cities in the dataset. As the size of the house increases (specifically, by an average of 1672.50 sq. ft.), the security deposit is expected to rise by ₹406,200. This is a logical correlation, as larger properties are more expensive to maintain and repair, justifying a higher deposit.
If a person rents a Villa or an Independent House, especially a large one located in Delhi, you should expect to pay the highest possible security deposit. These three factors—property type, location, and size—are the key drivers that landlords use to determine the amount of security they require.





