This repository is a complete database based on a simple interpretation of restaurant data relationships(The interpretation can be found below).
The exact SQL implementation code can be found in script.txt.
Other files create a website, called restaurant.html, where all the data in the database can be accessed.




INTERPRETATION:

Your database will store information about a family of restaurants with the requirements outlined as follows:

there are 4 different restaurants owned by the same company.  Each restaurant has a unique name, a unique URL and an address.
restaurants have employees which are one of a) management, b) delivery, c) chef, d) server.  All employees have a unique (among all restaurants) employee ID (an integer), a name and an email address.   Each employee works at only one restaurant.
each week the employee's schedule is stored which consists of a list of days, start times and end times.  No employee works two shifts on the same day of the week.  Historical data for schedules is not stored, just the current week's schedule.
each restaurant has an online menu offering food items that customers may order (think Door Dash).  Each food item is described by the name of the food ("fries") and a price (4.25).  Of course each restaurant may sell the same items either at the same or a different price.
customers are stored in the database using a unique identifier (their email address), a name (first name and last name), as well as a phone number and a delivery address.  Customers are added to the database before they have placed any orders.
all customers have an account which keeps track of payments made, the date on which the payment was made and the amount of credit that the customer has.  The account does not store information about the orders that have been made, only payments.
customers place orders from the restaurants.  Each order has a unique order ID (an integer).  We keep track of the items that were ordered, the total amount (price) of the order, the tip that was given by the customer for the order, the order placement time and the order delivery time.  We also keep track of who delivered the order to the customer.
these restaurants are in a small town and so we want to keep track of the relationships between the restaurant employees and the customers, just because we can!
chefs have different credentials such as those listed on this website.  For each chef we will store the various credentials that they have.
