# oo-many-many-practice

# Here's our domain:
  * Patient
  * Doctor
  * Appointment

# How is this modeled?
  * An appointment belongs_to a doctor
  * An appointment belongs_to a patient
  * A patient has_many appointments
  * A doctor has_many appointments
  * A patient has_many doctors through appointments
  * A doctor has_many patients through appointments

==============================================================

#OBJECTIVES
  * Draw this domain on a whiteboard or http://awwapp.com/
  * Build out the three classes and files from scratch (keep in mind the relationships)
  * Think about how the classes will interact -- how does a doctor know about their patients?
  * Use attr_reader, attr_writer, & attr_accessor
  * Create a run file with a single point of entry
  * Maintain single source of truth for all classes

==============================================================

#DELIVERABLES
  * DOCTOR
    * #initialize a doctor is initialized with a name and a specialty
    * a doctor cannot change their name, but can change their specialty
    * Doctor.all returns all instances of the doctor class
    * #appointments returns an array of all the appointment instances that belong_to a doctor
    * #patients return an array of all the patients that are associated with a doctor
    * #patient names return an array of just the names of said patients, not the full object
    ====== BONUS ======
    * Doctor.find_by_specialty takes in a specialty as an argument and finds a doctor by a given specialty
    * #reschedule_appointment takes in an appointment and a new date and changes the appointment's date

==============================================================
  * PATIENT
    * #initialize a patient is initialized with a name
    * a patient cannot change their name
    * Patient.all returns all instances of the patient class
    * #appointments returns an array of all the appointments associated with an instance of patient
    * #schedule_appointment creates a new appointment instance taking in a doctor and a time
    ====== BONUS ======
    * Patient.find_by_name takes in name as an argument and finds a patient by a given name
    * #find_doc finds a doctor by specialty -- utilizing the Doctor.find_by_specialty class method

==============================================================
  * APPOINTMENT
    * #initialize  an appointment is initialized with a date, a patient and a doctor
    * an appointment has corresponding methods for all three attributes
    * Appointment.all returns all instances of the appointment class

==============================================================
