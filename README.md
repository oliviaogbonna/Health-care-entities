Overview

This project presents an Entity-Relationship Diagram (ERD) for a healthcare management system. The ERD models key entities such as Patient, Provider, Appointment, Department, and Billing with clearly defined relationships and cardinality.

Entities & Attributes

PATIENT

Patient_ID (PK): Unique identifier

First_Name: Patient's first name

Last_Name: Patient's last name

DOB: Date of birth

Phone_Number: Contact information

PROVIDER

Provider_ID (PK): Unique identifier

First_Name: Provider’s first name

Last_Name: Provider’s last name

Specialty: Medical specialty

License_Number: Professional license number

APPOINTMENT

Appointment_ID (PK): Unique identifier

Appointment_Date: Date of appointment

Appointment_Time: Time of appointment

Status: Current status of the appointment

Reason_For_Visit: Purpose of the appointment

DEPARTMENT

Department_ID (PK): Unique identifier

Department_Name: Name of the department

Location: Location of the department

Phone_Number: Contact phone number

Operating_Hours: Hours of operation

BILLING

Billing_ID (PK): Unique identifier

Billing_Date: Date the bill was created

Total_Amount: Total cost for services provided

Payment_Status: Current status of payment

Payment_Method: Method used for payment

Relationships

PATIENT — APPOINTMENT (1:M): A patient may have zero or many appointments, each appointment belongs to exactly one patient.

PROVIDER — APPOINTMENT (1:M): A provider may conduct zero or many appointments, each appointment must have one provider.

DEPARTMENT — PROVIDER (1:M): A department may employ zero or many providers, each provider belongs to one department.

APPOINTMENT — BILLING (1:1): Each appointment generates exactly one billing record, and each billing record corresponds to one appointment.

Notation

This ERD uses Crow’s Foot notation to represent relationships between entities.

1 = One

M = Many

| = Mandatory

O = Optional

How to Use

Download or clone the repository to explore the ERD and understand how entities in a healthcare management system are related.

This ERD can be used as a foundational model for building a database schema or as a reference for healthcare management system design.
