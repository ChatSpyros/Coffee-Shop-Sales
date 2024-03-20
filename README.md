# Coffee-Shop-Sales
The project involves transaction records for Maven Roasters, a fictitious coffee shop operating out of three NYC locations. Dataset includes the transaction date, timestamp and location, along with product-level details.

## Business Problems 

•	How do sales vary by day of the week and hour of the day?

•	Are there any peak times for sales activity?

•	What is the total sales revenue for each month?

•	How do sales vary across different sore locations?

•	What is the average price/order per person?

•	Which products are the best-selling in terms of quantity and revenue?

•	How do sales vary by product category and type? 


## Data Cleaning 
The entire data cleaning process was conducted using Excel's Power Query feature.

##### 1. Identification of Missing Values:

- Utilizing Power Query, the dataset was loaded into Excel for examination.
- Each column was thoroughly inspected to identify any blanks or missing values.
- Power Query's filtering capabilities were leveraged to isolate records with missing values in each column.

##### 2. Verification of Data Formats:

-	For each column, the data format was examined to ensure appropriateness for the type of data it contained.
-	Date and time columns were scrutinized to verify consistency in format and resolve any discrepancies.
-	Numeric columns such as unit price were checked for numeric formatting, ensuring compatibility with mathematical operations.
-	Categorical columns like store ID and product ID were inspected to confirm adherence to predefined formats or codes.

 ##### 3. Standardization of Data Formats:

-	Data formats were standardized across columns to enhance consistency and facilitate analysis.
-	Date and time formats were standardized to a uniform structure, such as YYYY-MM-DD for dates and HH:MM:SS for times.
-	Categorical data, including store IDs and product categories, were standardized to ensure uniform representation throughout the dataset.


## Data Transformation

- [x]  Create a column to categorize by size of products (Large, Small, Regular):
A new column named "Product Size" is created based on the values in the "Product Details" column.
Using conditional logic, products are categorized into "Large," "Small," or "Regular" based on their size.
 - [x] Transform product details column:
The values "Rg," "LG," and "Sm" in the "Product Details" column are replaced with blank to remove the size indication at the end of each product detail.
Trim the column product details:
Leading and trailing spaces are removed from the "Product Details" column to ensure uniformity in formatting.
 - [x] Create a custom column Total Bill:
A new column named "Total Bill" is created by multiplying the "Transaction Quantity" and "Unit Price" columns.
This calculates the total cost of each transaction, considering the quantity and price of the product.
 - [x] Create a column for the transaction hour:
A new column named "Transaction Hour" is created to extract only the hour portion of the "Transaction Time" column.
The hour is represented as a whole number, indicating the hour of the day when each transaction occurred.
 - [x] Create a column name of month:
A new column named "Month Name" is created to extract the month component from the "Transaction Date" column.
The month name is derived from the date value, providing a categorical representation of the month.
 - [x] Create a column for the day of the week:
A new column named "Day of the Week" is created to extract the day of the week from the "Transaction Date" column.
The day of the week is derived from the date value, providing a categorical representation of the day of the week

## Key Takeaways 


-	Our analysis reveals discernible patterns in sales activity concerning the day of the week and hour of the day. Notably, we observe a pronounced preference for coffee during the hours of 8:00 to 10:00. This time frame consistently records the highest transaction volume and revenue generation across all days of the week.

-	An examination of sales patterns reveals that Saturdays and Sundays emerge as the days with the highest revenue and transaction volumes.


-	It is evident that Hell's Kitchen emerges as the store with the highest revenue among all locations. Following closely behind is the Astoria store, with Lower Manhattan ranking third in terms of revenue generation

-	After analyzing sales data for 29 products types, it's clear that Barista Espresso leads in sales volume, closely followed by Brewed Chai Tea and Hot Chocolate. Gourmet Brewed Coffee and Brewed Herbal Tea also perform well.

-	In assessing product category sales, coffee emerges as the clear frontrunner, demonstrating robust performance and significantly outperforming other categories. Following closely behind is tea, contributing substantially to overall sales. Bakery products maintain a solid position, while drinking chocolate trails at a noticeable distance




