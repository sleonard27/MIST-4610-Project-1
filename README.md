# MIST-4610-Project-1

## Team Name:
71552 Group 7

## Team Members:
1. Leonard, Sean [@sleonard27] (https://github.com/sleonard27)
2.


## Problem Description:
This project displays a database management system for a restaurant. The system is built to efficiently handle and organize restaurant operations, including orders, payments, menu items, customers, and staff management. By developing a structured and optimized database, we aim to make it useful for management decisions and thus ultimately enhancing operational efficiency. 

## Data Model:
This data model represents the operational framework of a restaurant, capturing details about orders, menu items, payments, staff, and table assignments. The Order entity serves as the core of the model, storing the order identifier, date, total price, and links to the assigned table and server, enabling the restaurant to track customer orders comprehensively. The Food and Drink entities hold the restaurant’s menu items, including names, descriptions, and prices, and are connected to orders through the Food_Order and Drink_Order entities, which record the specific items and quantities ordered to ensure accurate fulfillment. The Table entity manages seating arrangements by tracking the number of customers and the assigned server, while the Server entity stores staff details such as name, salary, and phone number, linking servers to both tables and orders for workforce management. The Payment and Split_Payment entities handle transaction processing, with Payment logging the total amount and order details, and Split_Payment allowing for flexible bill splitting with various payment types and dates, accommodating diverse customer preferences. The relationships between these entities ensure efficient management of daily restaurant operations. 
The Order entity acts as the foundation of the data model, linking to the Table entity in a one-to-many relationship where a table can have multiple orders, but each order is tied to a single table, facilitating order tracking by location. The Server entity also relates to the Order entity in a one-to-many relationship, where a server can handle multiple orders, but each order is assigned to one server, supporting staff performance monitoring. The Table entity connects to the Server entity in a one-to-many relationship, allowing a server to manage multiple tables, though each table is assigned to one server for clear responsibility. The Order entity has a many-to-many relationship with both Food and Drink entities through the Food_Order and Drink_Order junction tables, where an order can include multiple items and an item can appear in multiple orders, with quantities tracked for precision. The Order entity links to the Payment entity in a one-to-one relationship, ensuring each order has a corresponding payment, while the Payment entity connects to the Split_Payment entity in a one-to-many relationship, enabling a payment to be divided into multiple splits, each tied to one payment for flexible billing. These relationships collectively support the restaurant’s ability to manage orders, staff, and finances effectively.
![Data Model](https://raw.githubusercontent.com/sleonard27/MIST-4610-Project-1/f0dece3f3ac559225a8c3ff18d17315272cfe6ea/Screenshot1.png)
## Data Dictionary:

## Queries:

## Database information:

Name of the database: ha_group7_crn71552

All queries are bookmarked through stored procedures and can be called using this format: CALL TP_Qx(); where 'x' is the query number.

