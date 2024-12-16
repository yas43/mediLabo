MediLabo 
Built With
Front End
Back end
Java 21: High-performance language for backend development.
Spring Boot: Framework for building microservices.
Spring Cloud Gateway: Used for routing and filtering requests to microservices.
Spring Security: 

Database
MongoDB: NoSQL database used to store patient prescriptions.
postgresql:  used for  patient data 

Architecture Overview

Gateway: A Spring Cloud Gateway that handles routing of requests to the appropriate microservices .
Patient microservice: Manages patient data, posygresql database .
Patient-history microservice: Manages medical records, using MongoDB for data storage.
Patient-historyAnalyse: microservice: Analyzes patient data to evaluate their risk for Type 2 diabetes.
Frontend: The user interface is built thymeleaf template.

This architecture allows for separation of concerns.

Getting Started
There are two primary ways to get started with the MediLabo app: using Docker or installing it manually.

Run App with Docker

Run docker compose

Manually install app
If you prefer to install and run the app manually, follow these steps:

Clone the Project:

Set Up the Backend:
Java 21 is installed on your machine.

Set up the databases:
The 'Patient_info microservice' uses an postgreql database .
Set Up MongoDB:
Install and run a MongoDB server locally.
 MongoDB database 
Once the application is up and running, navigate to http://localhost:8083 to start using the app.

The default credentials to log in to the app are:

Username: user
Password: user
The user interface allows you to:

View a list of patients and their risk for Type 2 diabetes based on the provided patient data.
Edit a patient’s data or add a new patient.
Add a new note (medical record) for a patient.
