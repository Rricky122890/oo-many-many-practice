# oo-many-many-practice

# Here's our domain:
  * Donation
  * Donor
  * Charity

# How is this modeled?
  * What's the relationship between a Donor and an Donation?
  * A Charity and an Donation?
  * A Donor and a Charity?

==============================================================

#OBJECTIVES
  * Draw this domain on a whiteboard or http://awwapp.com/
  * Build out the three classes and files from scratch (keep in mind the relationships)
  * Think about how the classes will interact -- how does a Charity know about their Donors?
  * Use attr_reader, attr_writer, & attr_accessor
  * Create a run file with a single point of entry
  * Maintain single source of truth for all classes

==============================================================

#DELIVERABLES
  * Charity
    * #initialize a charity is initialized with a name and a category
    * a charity can change their name and category

  * CLASS METHODS
    * Charity.all returns all instances of the charity class

  * INSTANCE METHODS
    * #donations returns an array of all the order instances that belong_to a charity
    * #donors return an array of all the customer that have made an donations to the charity
    * #donor_names return an array of just the names of said donors, not the full object

    ====== BONUS ======
    * Charity.find_by_category takes in a category as an argument and finds a charity by a given category

==============================================================

  * DONOR
    * #initialize a donor is initialized with a name
    * a donor cannot change their name

  * CLASS METHODS
    * Donor.all returns all instances of the donor class

  * INSTANCE METHODS
    * #donations returns an array of all the donations associated with an instance of donor
    * #make_donation creates a new donation instance taking arguments of a Charity and an amount

    ====== BONUS ======
    * Donor.find_by_name takes in name as an argument and finds a donor by a given name

==============================================================

  * DONATION
    * #initialize a donation is initialized with a donor, a charity and an amount
    * a donation has corresponding attribute readers & writers for all three attributes
    * Donation.all returns all instances of the donation class

==============================================================
