# Robot-Controller-and-Assistant 
This repository contains Task 1 Robot Arm(submitted on 6/30), Task 2 Robot Base(submitted on 7/8), and Task 3 IBM Watson(submitted on 7/15)  in IoT path at Smart Methods summer training.  

The index.php file has the interface for the conroller made using bootstrap 4.  
The interface has 6 motors each with a range of 180, an on/off switch to turn the motros on/off, and a save button that submits the changes into the database.  
The interface also has 5 direction buttons that guides the robot. Each time a direction button is pressed the database gets updated.  
At the beging of the file there's a php code that retrieves the values of the motors, the switch, and the active direction from the database and puts the values on the page.  

The includes/connector.php file makes the connection to the database.  
The database was made using MySQL through XAMPP.
the database has two tabels motors, and direction.  
the motor table has three columns: motor(motor number), angle(0-180), and status(on/off).
the direction table has 5 columns: forward, right, backward, left, stop.  

The includes/save.php handles the submition of the values from the web page to the database, after clicking the save button.  

The includes/direction.php handles the submittion of the value of the active direction to the database.  

controller.sql is the extracted database from phpMyAdmin used for the tasks.  

Receptionist.JSON contains an IBM Watson assistant custom made to respond to inquiries about the controller.  

- Abdullah Alsaleh
- KFUPM ID: 201637180
