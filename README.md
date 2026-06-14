# assignment-1-hospital-database

The aim of this project was to develop a hospital database looking at the different relationships between hospitals, doctors, patients and prescriptions with the data being included from a pre-given dataset. 

## Database:
contains hospitals.csv, doctors.csv, patients.csv and prescriptions.csv.

Four tables were created for these four components of the database and the same SQL schema was used, with the columns being adjusted for each component.

## Hospitals table:
- hospital_id (Primary key)
- name
- address
- size
- type
- accreditation_status

## Doctors table:
- doctors_id (Primary key)
- name
- date_of_birth
- address
- role
- hospital_id (Foreign key ref doctors)

## Patients table:
- person_id (Primary Key)
- name
- date_of_birth
- address
- role 
- doctor_id (Foreign key ref doctors)

## Prescriptions table:
- prescription_id (Primary key)
- patient_id (Foreign key ref patients)
- doctor_id (Foreign key ref doctors)
- medication
- prescription date
 

## SQL SCHEMA
Below is an example of the SQL schema used to create the table for doctors
CREATE TABLE doctors

(

doctor_id  INT unsigned NOT NULL AUTO_INCREMENT,

name  VARCHAR(150) NOT NULL,

date_of_birth  date NOT NULL,

address  VARCHAR(150) NOT NULL,

role  VARCHAR(150) NOT NULL,

hospital_id  VARCHAR(150) NOT NULL,

PRIMARY KEY  (doctor_id)

);



## Queries Completed:
1. List all doctors based at a particular hospital. (Purpose: We're able to see the link between doctors and hospitals which is a 1-many relationship as one hospital has many doctors.)
2. List all prescriptions for a particular patient, ordered by the prescription date. (Purpose: Patient-prescription relationship is a 1- many, meaning one patient might have 2 or more prescriptions so running this query allows us to see all the prescriptions for a particular patient).
3. List all prescriptions that a particular doctor has prescribed. (Purpose: Doctor-prescription relationship is also a 1-many relationship, meaning one doctor can prescribe many medications, which will be shown when this query is ran.)
4. Add a new patient to the database, including being registered with one of the doctors. (Purpose: Shows the functionality of the patients table and that they can be assigned a doctor.)
5. Identify which doctor has made the most prescriptions. (Purpose: Re-iterates the 1-Many relationship between doctor-prescription but this time we can see which doctor has prescribed the most medications.)
6. List all doctors at the hospital with biggest size. (Purpose: It shows us the doctors working at the biggest hospitals.)

## SQL FEATURES USED
- A few of the features used included were:
- CREATE TABLE 
- INSERT
- SELECT *FROM
WHERE 

## Files:
- README.md
- SQL QUERIES for hospitals database
- hospitaldatabase.mysql
- entity relationship diagram.png


