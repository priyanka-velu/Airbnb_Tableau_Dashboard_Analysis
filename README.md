# Airbnb Tableau Dashboard

## Project Overview
Analyzed Airbnb metrics and created an Airbnb Tableau Dashboard to guide Airbnb investors in making data-driven decisions to maximize profitability and optimize their Airbnb listings.

Interactive Tableau Dashboard can be found [here](https://public.tableau.com/views/AirBnBTableauFinalProject/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link).

![Dashboard 1 (3)](https://github.com/user-attachments/assets/42938910-d13f-4b9b-8b36-54d536a30001)

## Resources
1. Data Source:
- [Kaggle](https://www.kaggle.com/datasets/airbnb/seattle)
- calender.csv
- listings.csv
- reviews.csv

2. Software:
- Microsoft Excel
- Tableau

## Main Objectives
1. **Pricing Analysis**:
   - Determine the average price per zip code.
   - Analyze the average price based on the number of bedrooms.

2. **Revenue Insights**:
   - Examine revenue trends throughout the year.
   - Identify the best times to list properties for maximum income.

3. **Competition Assessment**:
   - Evaluate the distribution of Airbnb listings by the number of bedrooms.
   - Identify bedroom categories with the highest and lowest competition.

4. **Geographical Trends**:
   - Highlight geographical variations in pricing.
   - Assess how location impacts rental prices and occupancy rates.

## Sheet 1: Average Price per Zipcode

![Screenshot 2024-07-20 171611](https://github.com/user-attachments/assets/7ffe6287-13aa-4fd2-a834-6edeb2cb3889)

**Question 1: Which zip codes have the highest average Airbnb prices?**
- **Answer:** By analyzing the average price per zip code, we can identify that zip codes with the highest average Airbnb prices include 98134, 98119, and 98101. Typically, these are zip codes located in prime areas with high demand, such as downtown Seattle or neighborhoods close to major attractions and business districts.

**Question 2: How does the average price vary between different zip codes?**
- **Answer:** The average price per zip code varies significantly, reflecting differences in location desirability, property types, and amenities. For instance, zip codes with luxury properties or those near tourist hotspots, such as zip codes of 98134 or 98119, tend to have higher average prices compared to suburban or less central areas, such as zip codes of 98125 or 98133.

## Sheet 2: Price by Zipcode (Map)

![Screenshot 2024-07-20 171651](https://github.com/user-attachments/assets/83665de3-78cc-4a71-80bc-5a870baddf00)

**Question 1: What are the geographical trends in Airbnb pricing across the city?**
- **Answer:** The map visualization reveals that Airbnb prices are generally higher in central and coastal areas, where proximity to attractions, restaurants, and public transportation is greater. Outlying areas tend to have lower prices, suggesting lower demand or fewer premium properties. We observe this when zip code 98134 is central and coastal compared to zipcodes 98125 and 98133, which are located in the outermost area.

## Sheet 3: Revenue for Year

![Screenshot 2024-07-20 171718](https://github.com/user-attachments/assets/16720f3a-1ab3-4f6e-baf6-eab9aae3954f)

**Question 1: Which months generate the highest Airbnb revenue?**
- **Answer:** The data shows that revenue peaks during the summer months, particularly from May to August during summer vacation. The revenue also peaks again during the months of November and December dure to the Holiday breaks. Both of these periods aligns with the tourist season and favorable weather, making it the most lucrative time to list an Airbnb property.

**Question 2: How does seasonality affect Airbnb revenue?**
- **Answer:** Revenue fluctuates throughout the year, with a noticeable drop in the winter months (January to March) and a peak in the summer. This seasonality suggests that property owners should adjust their pricing and availability to capitalize on high-demand periods and manage occupancy during slower months.

**Challenge:** 
- Originall, there was a large drop in Revenue after December. This is because there was a value being accounted for in January for next year.
- We can eliminate this data by filtering out the Date to WEEK and filter up to December 31st instead of January 1st.

## Sheet 4: Average Price of Bedrooms

![Screenshot 2024-07-20 171743](https://github.com/user-attachments/assets/212b7621-6526-4c97-b458-8279f140a60f)

**Question 1: How does the number of bedrooms affect the average price of an Airbnb listing?**
- **Answer:** There is a clear positive correlation between the number of bedrooms and the average price of an Airbnb listing. Properties with more bedrooms, especially those with five or more, command significantly higher prices, reflecting their ability to accommodate larger groups and offer more amenities.

**Question 2: What is the optimal number of bedrooms for maximizing rental income?**
- **Answer:** While larger properties with more bedrooms generate higher prices, they also cater to a niche market. The optimal number of bedrooms for maximizing rental income, balancing high demand and competitive pricing, appears to be between two and three bedrooms. This size appeals to a broad range of guests, including small families and groups of friends.

## Sheet 5: Discount Count of Bedroom Listings

![Screenshot 2024-07-20 171807](https://github.com/user-attachments/assets/46c5c20f-72ea-4f5f-bb58-61cc6875a0ba)

**Question 1: How does the competition vary by the number of bedrooms in Airbnb listings?**
- **Answer:** Competition is highest for one-bedroom listings, with 1,811 such properties in the market. As the number of bedrooms increases, the competition decreases, indicating fewer listings available for larger properties. This trend suggests that investors in larger properties may face less competition.

**Question 2: Which bedroom categories offer the least competition and potentially higher pricing power?**
- **Answer:** Listings with more bedrooms, particularly those with four or more, face significantly less competition. These categories offer property owners the opportunity to leverage higher pricing power due to the limited availability and the premium nature of larger accommodations.
