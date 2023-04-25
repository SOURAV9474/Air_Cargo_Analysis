# *Air Cargo Analysis*

**DESCRIPTION :-**

Air Cargo is an aviation company that provides air transportation services for passengers and freight. Air Cargo uses its aircraft to provide different services with the help of partnerships or alliances with other airlines. The company wants to prepare reports on regular passengers, busiest routes, ticket sales details, and other scenarios to improve the ease of travel and booking for customers.

 

**Project Objective :-**

You, as a DBA expert, need to focus on identifying the regular customers to provide offers, analyze the busiest route which helps to increase the number of aircraft required and prepare an analysis to determine the ticket sales details. This will ensure that the company improves its operability and becomes more customer-centric and a favorable choice for air travel.

**Note :-** You must download the dataset from the course resource section in the LMS and create the tables to perform the above objective.

**Dataset description :-**

Customer :- Contains the information of customers

    1. customer_id – ID of the customer
    2. first_name – First name of the customer
    3. last_name – Last name of the customer
    4. date_of_birth – Date of birth of the customer
    5. gender – Gender of the customer

passengers_on_flights :- Contains information about the travel details

    1. aircraft_id – ID of each aircraft in a brand
    2. route_id – Route ID of from and to location
    3. customer_id – ID of the customer
    4. depart – Departure place from the airport
    5. arrival – Arrival place in the airport
    6. seat_num – Unique seat number for each passenger
    7. class_id – ID of travel class
    8. travel_date – Travel date of each passenger
    9. flight_num – Specific flight number for each route

ticket_details :- Contains information about the ticket details
    
    1. p_date – Ticket purchase date
    2. customer_id – ID of the customer
    3. aircraft_id – ID of each aircraft in a brand
    4. class_id – ID of travel class
    5. no_of_tickets – Number of tickets purchased
    6. a_code – Code of each airport
    7. price_per_ticket – Price of a ticket
    8. brand – Aviation service provider for each aircraft

routes :- Contains information about the route details

    1. Route_id – Route ID of from and to location
    2. Flight_num – Specific fight number for each route
    3. Origin_airport – Departure location
    4. Destination_airport – Arrival location
    5. Aircraft_id – ID of each aircraft in a brand
    6. Distance_miles – Distance between departure and arrival location

**Following operations should be performed :-**

1. Create an ER diagram for the given airlines database.
2. Write a query to create route_details table using suitable data types for the fields, such as route_id, flight_num, origin_airport, destination_airport, aircraft_id, and distance_miles. Implement the check constraint for the flight number and unique constraint for the route_id fields. Also, make sure that the distance miles field is greater than 0.
3. Write a query to display all the passengers (customers) who have travelled in routes 01 to 25. Take data  from the passengers_on_flights table.
4. Write a query to identify the number of passengers and total revenue in business class from the ticket_details table.
5. Write a query to display the full name of the customer by extracting the first name and last name from the customer table.
6. Write a query to extract the customers who have registered and booked a ticket. Use data from the customer and ticket_details tables.
7. Write a query to identify the customer’s first name and last name based on their customer ID and brand (Emirates) from the ticket_details table.
8. Write a query to identify the customers who have travelled by Economy Plus class using Group By and Having clause on the passengers_on_flights table.
9. Write a query to identify whether the revenue has crossed 10000 using the IF clause on the ticket_details table.
10. Write a query to create and grant access to a new user to perform operations on a database.
11. Write a query to find the maximum ticket price for each class using window functions on the ticket_details table.
12. Write a query to extract the passengers whose route ID is 4 by improving the speed and performance of the passengers_on_flights table.
13. For the route ID 4, write a query to view the execution plan of the passengers_on_flights table.
14. Write a query to calculate the total price of all tickets booked by a customer across different aircraft IDs using rollup function.
15. Write a query to create a view with only business class customers along with the brand of airlines.
16. Write a query to create a stored procedure to get the details of all passengers flying between a range of routes defined in run time. Also, return an error message if the table doesn't exist.
17. Write a query to create a stored procedure that extracts all the details from the routes table where the travelled distance is more than 2000 miles.
18. Write a query to create a stored procedure that groups the distance travelled by each flight into three categories. The categories are, short distance travel (SDT) for >=0 AND <= 2000 miles, intermediate distance travel (IDT) for >2000 AND <=6500, and long-distance travel (LDT) for >6500.
19. Write a query to extract ticket purchase date, customer ID, class ID and specify if the complimentary services are provided for the specific class using a stored function in stored procedure on the ticket_details table.
    
    Condition :-

        If the class is Business and Economy Plus, then complimentary services are given as Yes, else it is No
20. Write a query to extract the first record of the customer whose last name ends with Scott using a cursor from the customer table.
