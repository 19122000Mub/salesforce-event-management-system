# Salesforce Event Management System

## Overview

This project was developed in Salesforce CRM to manage events, sessions, speakers, attendees, registrations, and feedback.

## Objects Used

* Event
* Session
* Speaker
* Attendee
* Feedback
* Event Registration

## Relationships

* Event → Session (Master-Detail)
* Speaker → Session (Lookup)
* Session → Feedback
* Event Registration (Junction Object)

## Skills Demonstrated

* Salesforce CRM
* Data Modeling
* SOQL
* Lookup Relationships
* Master-Detail Relationships
* Aggregate Functions

## Sample SOQL Queries

### Average Rating Per Session

SELECT Session__r.Name, AVG(Rating__c)
FROM Feedback__c
GROUP BY Session__r.Name

### Attendees Registered for Multiple Events

SELECT Attendee__c, COUNT(Id)
FROM EventRegistration__c
GROUP BY Attendee__c
HAVING COUNT(Id) > 1

## Learning Outcomes

* Salesforce CRM Fundamentals
* Object Relationships
* Data Modeling
* SOQL Query Writing
* Aggregate Functions
