# assignment-1-hospital-database
<!--
The aim of this project was to develop a hospital database looking at the relationships between hospitals, doctors, patients and prescriptions and the data was pre-given. 

Database:
contains hospitals.csv, doctors.csv, patients.csv and prescriptions.csv.
Four tables were created for these four components of the database and the same SQL schema was used, with the columns being adjusted for each component.

Hospitals table:
- the columns were as follows: hospital_id, name, address, size, type and accreditation status.
Doctors table:
- the columns were as follows: doctors_id, name, date_of_birth, address, role and hospital_id.
Patients table:
- the columns were as follows: person_id, name, date_of_birth, address, role and doctor_id.
Prescriptions table:
- the columns were as follows: prescription_id, patient_id, doctor_id, medication, prescription date.
 


An example of the SQL schema used to create the table for doctors
CREATE TABLE doctors

(

doctor_id               INT unsigned NOT NULL AUTO_INCREMENT,

name                    VARCHAR(150) NOT NULL,

date_of_birth           date NOT NULL,

address                 VARCHAR(150) NOT NULL,

role                    VARCHAR(150) NOT NULL,

hospital_id             VARCHAR(150) NOT NULL,

PRIMARY KEY    (CustomerID)

);



Queries Completed:
1. List all doctors based at a particular hospital.
2. List all prescriptions for a particular patient, ordered by the prescription date.
3. List all prescriptions that a particular doctor has prescribed.
4. Add a new patient to the database, including being registered with one of the doctors.
Identify which doctor has made the most prescriptions.
List all doctors at the hospital with biggest size.

SQL FEATURES USED
- A few of the features used included were:
- CREATE TABLE 
- INSERT
- SELECT *FROM

Files:
- README.md
- hospitaldatabase.mysql
- entity relationship diagram.png


