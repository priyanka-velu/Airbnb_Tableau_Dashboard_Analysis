# Airbnb Tableau Dashboard

## Project Overview
Creating an Airbnb Dashboard on Tableau to answer business questions related to consumers

Link to the [Airbnb Tableau Dashboard](https://public.tableau.com/views/AirBnBTableauFinalProject/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link) 

## Resources
1. Data Source:
- [Kaggle](https://www.kaggle.com/datasets/airbnb/seattle)
- calender.csv
- listings.csv
- reviews.csv

2. Software:
- Tableau

## Download data and JOIN table
- download useful data

- may not use listings.csv since useless data
- reviews: understand which IDs match, could be called differenly
- calender: IDs match, date and price

In Tableau: Microsoft Excel, open project
- start with listings with IDs, locations, update automatically
- OPEN table listings ID
- INNER JOIN table calender ON listing ID (double check using the number of rows 100 rows)
- INNER JOIN table reviews ON listing ID (2 million rows)

find the correct ID so that it matches properly so that you pull in the correct data

## Objective

How expensive is each zip code?

Use case for data
i would like to start an Airbnb business, where should buy a home, put it on Airbnb and rent it out?
What are all the factors I should be looking for?
bedrooms, location, how much price should i charge?

goals:
gain more profit
find our stakeholder find a really good Airbnb

## Sheet 1: Price per Zipcode
- Tableau seperates by character and numeric variables
  
-  find out the average price of each zip code
-  zip code on x axid = columns
-  price on y axis = rows

- add zipcode
- exclude NULL values
- add price, change to AVG price,
- order it from largest to smallest with icon

- color it by adding zipcode: color


## Sheet 2: Price by Zipcode (Map)

- location data, use same zipcode
- zipcode in columns
- click the map on the right side to show the codes

- color it by zipcode: color

- text by zipcode: label (what code is it?)

- add price (average): label
- look at the location itself


## Sheet 3: Revenue for Year

- im thinking about listing the airbnb but also live in it so i want to know the best times to put it on the market for people to use?
- when are people spending the most amount of time in airbnbs?

- date in columns (seperate by week)
- price(calender)

- challenge: huge drop at dec because only one data and get the sum so need to get rif of it
- filter WEEK(Date) bring it back to dec 31st instead of jan 1st

- findings
- not a lot of people travel during the beginning of the year
- i would suggest renting our your airbnb during the summer  from may to the end of the year

## Sheet 4: Average Price of Bedrooms

what will affect the price of the bedrooms?
How many bedrooms and how much they cost?

Bedrooms 
- numeric bedrooms will get the SUM automatically (meaure: CNTD) for count distinct for 1, 2, 3, 4 bedroooms
- convert numeric bedroom to dimenstion through right click
- dimension allows us to get the count themselves, not the average or sum

- get the AVG(price) of each TYPE of bedroom
- findings: we found that 6-bedroom airbnbs bring the most amount of money because it costs a lot more and a hgiher return on investment the higher he goes

- add label of price on bar graph (price: label), change to AVERAGE price

## Sheet 5: Discount Count of Bedroom Listings

What does his competition look like?

Bedrooms in rows
use ID to represent each airbnb: attribute: measure: count distinct: text
- convert into a numeric

- there are 1,811 1-bedroom, 482 2 bedroom
- so the higher the number of bedrooms, the LESS competition there is


## Create the Dashboard
- change size to automatic to use all of the space
- add them all
