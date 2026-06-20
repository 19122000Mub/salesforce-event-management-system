# Salesforce Event Management System

A Salesforce CRM project developed to manage Events, Sessions, Speakers, Attendees, Registrations, and Feedback.

## Skills Used

* Salesforce CRM
* SOQL
* Data Modeling
* Lookup Relationships
* Master-Detail Relationships

## Objects

* Event
* Session
* Speaker
* Attendee
* Feedback
* Event Registration

## Sample Query

SELECT Session__r.Name, AVG(Rating__c)
FROM Feedback__c
GROUP BY Session__r.Name
