# StreetFix
This repository contains the ServiceNow files of StreetFix application. 

**Do not edit the files in this repository outside of an instance of ServiceNow.**

Tracking of Issues/Damages in The Streets
You have received a work to create a functioning street-issues tracking for the city, so that they can fix them as soon as possible and have an overview of the status of the city streets.
Objective:
You must create the following tables, each having the attributes written thereunder: 
•	“City” table
o	City ID
o	Name
o	Country (Simple choice list)
•	“District” table
o	District ID
o	Name
o	Country (Simple choice list)
o	City (Referenced to the “City” table, dependent on the country)
•	“Street” table 
o	Street ID
o	Name
o	City (Referenced to the “City” table)
o	District (Referenced to the “District” table, dependent on the city field hereupon)
o	length
o	Number of lanes 
o	Crosses border or not
o	Importance
•	“Employee” table 
o	Employee ID
o	Name
o	Address
o	Phone number
o	Issues counted by this employee
o	Salary
o	Assigned District (Referenced to the “District” table)
o	
•	“Issue” table
o	Issue ID
o	Country (Simple choice list)
o	City (Referenced to the “City” table, dependent on the country)
o	Street (Referenced to the “Street” table, dependent on the city)
o	Impact
o	Urgency
o	Priority of issue (Automatically populated in a value between 1 and 10 according to impact, urgency and the importance of the street and if the street crosses borders or not and how many lanes the street has) 
o	Reported by employee (Referenced to the “Employee” table)

