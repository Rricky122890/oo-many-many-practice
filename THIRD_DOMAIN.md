# oo-many-many-practice

For this practice, we'll be building a concert app. In this domain, a `Fan` has many `Band`s, through a `Show`. A `Band` can play in many `Show`s and is connect to many `Fan`s through shows.

Sketch out the domain on a white board to help visualize the relationships.

==============================================================

#OBJECTIVES
  * Draw this domain on a whiteboard or http://awwapp.com/
  * Build out the three classes and files from scratch (keep in mind the relationships)
  * Think about how the classes will interact -- how does a Band know about their Fans?
  * Use attr_reader, attr_writer, & attr_accessor
  * Create a run file with a single point of entry
  * Maintain single source of truth for all classes

==============================================================

#DELIVERABLES
  * BAND
    * Band#initialize a Band is initialized with a name and a genre
    * a band can change their name and genre
    * Band.all returns all instances of the band class

    * Band#shows returns an array of all the show instances that belong_to a band
    * Band#fans return an array of all the fans that have attended a band's show
    * Band#fan_emails return an array of just the emails of the band's fans, not the full object
    * Band.find_by_genre(genre) finds the first band by a given genre

==============================================================

  * FAN
    * Fan#initialize a fan is initialized with a name and an email
    * Fan.all returns all instances of the fan class
    * Fan#shows returns an array of all the shows this fan has attended
    * Fan#go_to_show(band, date) creates a new show instance taking arguments of a band and a date

==============================================================

  * SHOW
    * Show#initialize -- what does a show need to be initialized?
    * Show.all returns all instances of the show class

==============================================================
