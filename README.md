# Hotel-Booking-Analysis

# Objective
We are provided with a hotel bookings dataset.

Out main objective is perform EDA on the given dataset and draw useful conclusions about general trends in hotel bookings and how factors governing hotel bookings interact with each other.

# Dataset
We are given a hotel bookings dataset. This dataset contains booking information for a city hotel and a resort hotel. It contains the following features.

- hotel: Name of hotel ( City or Resort)
- is_canceled: Whether the booking is canceled or not (0 for no canceled and 1 for canceled)
- arrival_date_year: Year of arrival
- arrival_date_month: month of arrival
- arrival_date_week_number: week number of arrival date.
- arrival_date_day_of_month: Day of month of arrival date
- children: No. of children in single booking record.
- meal: Type of meal chosen 
- country: Country of origin of customers (as mentioned by them)

###### Total number of rows in data: 119390
###### Total number of columns: 32

# Data Cleaning and Feature Engineering
###### 1. Removing Duplicate rows
All duplicate rows were dropped.

###### 2. Handling null values
Null values in columns company and agent were replaced by 0.
Null values in column country were replaced by 'others'.
Null values in column children were replaced by the mean of the column.

###### 3. Converting columns to appropriate data types
Changed data type of children, company, agent to int type.
Changed data type of reservation_status_date to date type.

###### 4. Removing outliers
One outlier was found in the adr column. Simply dropped it.

###### 5. Creating new columns
Created new column total_stay by adding stays_in_weekend_nights+stays_in_week_nights.
Created new column total_people by adding adults+children+babies.

## To discuss the analysis of given hotel bookings data set from 2015-2017.

###### We’ll be doing analysis of given data set in following ways :

###### 1. Hotel wise analysis

###### 2. Booking cancellation analysis

# Hotel Wise Analysis
While doing univariate analysis of given hotel booking dataset, we answered following questions:

1. Which meal is preferred by most Customer?
2. Which Hotel is booked most?
3. From which country most of the customers are coming?

# Booking Wise Analysis 
While doing booking analysis of given hotel booking dataset, we answered following questions:

1. Which hotel has higher bookings cancellation rate?
2. Which month have most Guest?
3. Which month is best for booking Hotel?
4. Which one is booking Hotel most(Single, Couple, Married)?


# Conclusion
We tried to answer following questions

1. Around 60% bookings are for City hotel and 40% bookings are for Resort hotel, therefore City Hotel is busier
than Resort hotel.

2. Most loving BB type food either from City or Resort Hotels.

3. Most of the guests came from european countries, with most no. of guest coming from Portugal.

4. Almost 30% of bookings are cancelled.

5. Most number of guest comes in month of August.

6. July- August are the most busier and profitable months for both of hotels.

7. Couples are the most common guests for hotels, hence hotels can plan services according to couples needs  to increase revenue.

And many more conclusions.
# Challenges
1. There was a lot of duplicate data.

2. Data was present in wrong datatype format.

3. Choosing appropriate visualization techniques to use was difficult.

4. A lot of null values were there in the dataset.
