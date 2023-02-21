# EDA-Capstone-Project-1
In this hotel booking analysis project, we explored the reasons that are governing the overall bookings in the hotels and also suggested the ideas to improve the business of the hotels. Hotel industry is a volatile industry and the bookings in hotels depending on the variety of factors such as type of hotels, customers(Transient Party,Contract,Transient,Group), month, special requests, carparkings, meal type etc. We analyzed the data provided and found the insights that help to increase the average revenue of the hotels. 

The hotel booking dataset has total 32 columns and 119390 rows. The data contains the booking related information of two hotels : City Hotel and Resort Hotel. The data regarding their cancellations,revenue etc, is also provided to create the insights for to meet the customer reuirements and increasing the hotel revenue.
Variables:
Hotel : H1= Resort Hotel , H2=City Hotel
is_cancelled : If the booking was cancelled(1) or not(0)
lead_time : Number of days that elapsed between the entering date of the booking into the PMS and the arrival date
arrival_date_year : Year of arrival date
arrival_date_month : Month of arrival date
arrival_date_week_number : Week number for arrival date
arrival_dat_day : Day of arrival date
stays_in_weekend_nights : Number of weekend nights (Saturday or Sunday) the guest stayed or booked to stay at the hotel
stays_in_week_nights : Number of week nights (Monday to Friday) the guest stayed or booked to stay at the hotel
adults : Number of adults
children : Number of children
babies : Number of babies
meal : Kind of meal opted for
      BB - bed and breakfast,
      HB - half board, in which breakfast and dinner are included,
      FB - full board, in which breakfast, lunch and dinner are included,
      SC - self-catering (no meals are included).
country : Country code
market segment : Which segment the customer belongs to
Distribution_channel : How the customer accessed the stay- corporate booking/Direct/TA.TO
is_repeated_guest : Guest coming for first time or not
previous_cancellation : Was there a cancellation before
previous_bookings : Count of previous bookings
reserved_room_type : Type of room reserved
assigned_room_type : Type of room assigned
booking changes : Count of changes made to booking
deposit_type : Deposit type
agent : Booked through agent
days_in_waiting_list : Number of days in waiting list
customer_type : Type of customer
Describing the customer type:
      *   Transient Party- Transient Party type customers are those who are looking for short and often urgent hotel stays.
      *   Contract 
      *   Transient - Transient guests are customers are those who consist of individuals or groups that are occupying less than 10 rooms per night
      *   Group
adr : Average Daily Revenue
required_car_parking : If car parking is required
total_of_special_req : Number of additional special requirements
reservation_status : Reservation of status
reservation_status_date : Date of the specific status
total_stays : The sum of stays_in_weekend_nights and stays_in_week_nights. The amount of stay in hotel

From the data, it is clear that more nulls are present in "company" and "agent" columns. It is because many times the bookings may not be done using these two ways. So, intsead of dropping the values, we filled the misssing values with other value like zero. Since, the country column datatype is string the missing values here are replaced with other string data.There are also few nulls in children data so replace the nulls with mean of children's column. After cleaning the data, we added new columns like "total stay" for improving the analysis. From the correaltion we got the inference that revenue depends on the amount of stay of guests. The total stay and leap time also has slight positive correlation. The comparision between both the hotels is also done and we found that City Hotel has highest revenue and is providing more facilities than the resort hotel. 
