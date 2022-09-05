# Hotel-Booking-Analysis

Objective
We are provided with a hotel bookings dataset.

Out main objective is perform EDA on the given dataset and draw useful conclusions about general trends in hotel bookings and how factors governing hotel bookings interact with each other.

Dataset
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


- previous_cancellations: No. of previous canceled bookings.
- previous_bookings_not_canceled: No. of previous non-canceled bookings.
- reserved_room_type: Room type reserved by a customer.
- assigned_room_type: Room type assigned to the customer.
- booking_changes: No. of booking changes done by customers
- deposit_type: Type of deposit at the time of making a booking (No deposit/ Refundable/ No refund)
- agent: Id of agent for booking
- company: Id of the company making a booking
- days_in_waiting_list: No. of days on waiting list.
- customer_type: Type of customer(Transient, Group, etc.)
- adr: Average Daily rate.
- required_car_parking_spaces: No. of car parking asked in booking
- total_of_special_requests: total no. of special request.
- reservation_status: Whether a customer has checked out or canceled,or not showed 
- reservation_status_date: Date of making reservation status.

Total number of rows in data: 119390
Total number of columns: 32

Data Cleaning and Feature Engineering
(1) Removing Duplicate rows
All duplicate rows were dropped.

(2) Handling null values
Null values in columns company and agent were replaced by 0.
Null values in column country were replaced by 'others'.
Null values in column children were replaced by the mean of the column.

(3) Converting columns to appropriate data types
Changed data type of children, company, agent to int type.
Changed data type of reservation_status_date to date type.

(4) Removing outliers
One outlier was found in the adr column. Simply dropped it.

(5) Creating new columns
Created new column total_stay by adding stays_in_weekend_nights+stays_in_week_nights.
Created new column total_people by adding adults+children+babies.

To discuss the analysis of given hotel bookings data set from 2015-2017.

We’ll be doing analysis of given data set in following ways :

Hotel wise analysis

Booking cancellation analysis

Hotel Wise Analysis
While doing univariate analysis of given hotel booking dataset, we answered following questions:

Which meal is preferred by most Customer?
Which Hotel is booked most?
From which country most of the customers are coming?

Booking Wise Analysis 
While doing booking analysis of given hotel booking dataset, we answered following questions:

Which hotel has higher bookings cancellation rate?
Which month have most Guest?
Which month is best for booking Hotel?
Which one is booking Hotel most(Single, Couple, Married)?


Bivariate Analysis :
We tried to answer following questions

Around 60% bookings are for City hotel and 40% bookings are for Resort hotel, therefore City Hotel is busier
than Resort hotel.

Most loving BB type food either from City or Resort Hotels.

Most of the guests came from european countries, with most no. of guest coming from Portugal.

Almost 30% of bookings are cancelled.

Most number of guest comes in month of August.

July- August are the most busier and profitable months for both of hotels.

Couples are the most common guests for hotels, hence hotels can plan services according to couples needs  to increase revenue.

And many more conclusions.
Challenges
(1) There was a lot of duplicate data.
(2) Data was present in wrong datatype format.
(3) Choosing appropriate visualization techniques to use was difficult.
(4) A lot of null values were there in the dataset.


