# oo-many-many-practice

# Here's our domain:
  * Order
  * Restaurant
  * Customer

# How is this modeled?
  * What's the relationship between a customer and an order?
  * A restaurant and an order?
  * A customer and a restaurant?

==============================================================

#OBJECTIVES
  * Draw this domain on a whiteboard or http://awwapp.com/
  * Build out the three classes and files from scratch (keep in mind the relationships)
  * Think about how the classes will interact -- how does a restaurant know about their customers?
  * Use attr_reader, attr_writer, & attr_accessor
  * Create a run file with a single point of entry
  * Maintain single source of truth for all classes

==============================================================

#DELIVERABLES
  * Restaurant
    * #initialize a restaurant is initialized with a name and a cuisine
    * a restaurant can change their name and cuisine

  * CLASS METHODS
    * Restaurant.all returns all instances of the restaurant class

  * INSTANCE METHODS
    * #order returns an array of all the order instances that belong_to a restaurant
    * #customers return an array of all the customer that have made an order at the restaurant
    * #customer_names return an array of just the names of said customers, not the full object

    ====== BONUS ======
    * Restaurant.find_by_cuisine takes in a cuisine as an argument and finds a restaurant by a given cuisine

==============================================================
  * CUSTOMER
    * #initialize a customer is initialized with a name
    * a customer cannot change their name

  * CLASS METHODS
    * Customer.all returns all instances of the customer class

  * INSTANCE METHODS
    * #orders returns an array of all the orders associated with an instance of customer
    * #place_order creates a new order instance taking in a restaurant and a dish

    ====== BONUS ======
    * Customer.find_by_name takes in name as an argument and finds a customer by a given name
    * #fav_restaurant returns the restaurant that has the highest number of orders placed by the instance of customer

==============================================================
  * ORDER
    * #initialize an order is initialized with a restaurant, a customer and a dish
    * an order has corresponding attribute readers & writers for all three attributes
    * Order.all returns all instances of the order class

==============================================================
