# Airbnb Singapore

## Business Understanding
Assist a property owner in devising a strategy to optimize rental activities for maximum profit through the Airbnb marketplace.
1. How many competitors are there in each region?
2. How many properties are offered by competitors?
3. What type of property is most frequently rented by visitors to Singapore?
4. Which region has the highest number of rented properties?
5. Why do so many customers rent properties in the prime region? Is it near Merlion Park, a notable Singapore landmark?
6. What properties are offered by competitors in the prime region?
7. What type of property is most frequently rented by consumers in the prime region?
8. What is the review trend in the prime region from January 1, 2018, to September 22, 2022?
9. Which neighborhoods have the highest number of consumers in the prime region?
10. What is the average price of the top 10 most active lodgings?
11. What challenges will the owner face?

## Data Understanding
- Data of Airbnb Transaction from January 1, 2018, to September 22, 2022
- Data Source: DQLab
- There are 3 datasets, which are:
  - Listing data: 12 columns and 4161 rows
    - Unnamed: 0
    - id
    - name
    - host_id
    - host_name
    - neighbourhood
    - latitude
    - longitude
    - room_type
    - price
    - minimum_nights
    - availability_365
      
  - Neighbourhood data: 3 columns and 55 rows
    - Unnamed: 0
    - neighbourhood_group
    - neighbourhood
      
  - Reviews Data: 3 columns and 49695 rows
    - Unnamed: 0
    - listing_id
    - date

## Data Preparation
-	Python Programming Language
-	Packages: pandas, numpy, matplotlib, seaborn, calendar, plotly, geopy

## Data Cleansing
### Listing Data:
  - Removing Unnamed: 0 Column
  - Delete rows that have a value of 0 in the price column

### Neighbourhood Data:
  - Removing Unnamed: 0 Column

### Reviews Data:
  - Removing Unnamed: 0 Column
  - Changing the data type of the date column

## Exploratory Data Analysis
1. How many competitors are there in each region?
   ![image](https://raw.githubusercontent.com/luthfifathurrahman/Airbnb-Singapore/main/images/How%20many%20competitors%20are%20there%20in%20each%20region.png)
   The region with the most competitors is the Central Region, with 2556 lodgings.
2. How many properties are offered by competitors?
   ![image](https://raw.githubusercontent.com/luthfifathurrahman/Airbnb-Singapore/main/images/How%20many%20properties%20are%20offered%20by%20competitors.png)
   The most common property competitors offer is the Entire Home/Apt, with 2330 lodgings.
3. What type of property is most frequently rented by visitors to Singapore?
   ![image](https://raw.githubusercontent.com/luthfifathurrahman/Airbnb-Singapore/main/images/What%20type%20of%20property%20is%20most%20frequently%20rented%20by%20visitors%20to%20Singapore.png)
   The most common property type rented by customers is the Entire Home/Apt, with 33654 times.
4. Which region has the highest number of rented properties?
   ![image](https://raw.githubusercontent.com/luthfifathurrahman/Airbnb-Singapore/main/images/Which%20region%20has%20the%20highest%20number%20of%20rented%20properties.png)
   Customers prefer to rent properties in the nothern region with 22915 times.
5. Why do so many customers rent properties in the prime region? Is it near Merlion Park, a notable Singapore landmark?
   ![image](https://raw.githubusercontent.com/luthfifathurrahman/Airbnb-Singapore/main/images/Why%20do%20so%20many%20customers%20rent%20properties%20in%20the%20prime%20region%20Is%20it%20near%20Merlion%20Park%20a%20notable%20Singapore%20landmark.PNG)
   No, because the closest property from the Northern Region is 7.7 km away from Merlion Park. 
   ![image](https://raw.githubusercontent.com/luthfifathurrahman/Airbnb-Singapore/main/images/Why%20do%20so%20many%20customers%20rent%20properties%20in%20the%20prime%20region%20Is%20it%20near%20Merlion%20Park%20a%20notable%20Singapore%20landmark%201.png)
   The reason are that Northern Region has an average price that is affordable/cheaper than other regions and Northern Region is close to Malaysia.
6. What properties are offered by competitors in the prime region?
   ![image](https://raw.githubusercontent.com/luthfifathurrahman/Airbnb-Singapore/main/images/What%20properties%20are%20offered%20by%20competitors%20in%20the%20prime%20region.png)
   The most common property competitors offer in the northern region is the Entire Home/Apt with 656 lodgings
7. What type of property is most frequently rented by consumers in the prime region?
   ![image](https://raw.githubusercontent.com/luthfifathurrahman/Airbnb-Singapore/main/images/What%20type%20of%20property%20is%20most%20frequently%20rented%20by%20consumers%20in%20the%20prime%20region.png)
   The most rented property by customers in the Northern Region is an Entire Home/Apt with 21630 times.
8. What is the review trend in the prime region from January 1, 2018, to September 22, 2022?
   ![image](https://raw.githubusercontent.com/luthfifathurrahman/Airbnb-Singapore/main/images/What%20is%20the%20review%20trend%20in%20the%20prime%20region%20from%20January%201%2C%202018%2C%20to%20September%2022%2C%202022.png)
   ![image](https://raw.githubusercontent.com/luthfifathurrahman/Airbnb-Singapore/main/images/What%20is%20the%20review%20trend%20in%20the%20prime%20region%20from%20January%201%2C%202018%2C%20to%20September%2022%2C%202022%201.png)
   The busy periods are May through August and December. Due to the summer, Christmas, and New Year holidays.
9. Which neighborhoods have the highest number of consumers in the prime region?
   ![image](https://raw.githubusercontent.com/luthfifathurrahman/Airbnb-Singapore/main/images/Which%20neighborhoods%20have%20the%20highest%20number%20of%20consumers%20in%20the%20prime%20region.png)
   More customers are opting for properties in Woodlands. 9 properties out of the top 10 most active lodgings are in the woodlands neighbourhood.
10. What is the average price of the top 10 most active lodgings?
   ![image](https://raw.githubusercontent.com/luthfifathurrahman/Airbnb-Singapore/main/images/What%20is%20the%20average%20price%20of%20the%20top%2010%20most%20active%20lodgings.PNG)
11. What challenges will the owner face?
   ![image](https://raw.githubusercontent.com/luthfifathurrahman/Airbnb-Singapore/main/images/What%20challenges%20will%20the%20owner%20face.png)
   From 2018 to 2022, there wwas a crisis in 2020. Where there was a decrease in the number of customers by 13.43%, this decline was caused by the Covid-19 virus outbreak that hit the whole world. This resulted in the WHO giving an appeal for social distancing. Some countries also decided to close access in and out. The virus outbreak impacted some hosts/owners, as some hosts/owners had to close their businesses. This is evidenced by the cessation of operations of 446 lodgings after January 23, 2020.

## Recommendation
To generate maximum profit through the Airbnb marketplace in Singapore, a property owner should pay attention to these points:
- It is advisable to rent out a property in the form of a house or apartment.
- It is advisable to have a property in the Northern Region, Woodlands neighbourhood.
- It is recommended to set a price rate around 52.8 SGD.
- It is recommended to focus Marketing Campaign on May to August and December.
- It is advisable to prepare an emergency fund to deal with out-of-control risks such as the Covid-19 virus outbreak.
