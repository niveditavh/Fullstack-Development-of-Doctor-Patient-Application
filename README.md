# Doctor Patient Appointment Application

A basic full-stack application built using:

- **Frontend:** React
- **Backend:** Spring Boot
- **Database:** MySQL
- **ORM:** Spring Data JPA / Hibernate
- **Containerization:** Docker & Docker Compose

This project allows users to:

- Add Doctor
- Delete Doctor
- Add Patient
- Delete Patient
- Create Appointment
- Cancel Appointment
- Delete Appointment

---
When running the backend locally from IntelliJ or terminal:

React (localhost:3000)
|
v
Spring Boot (localhost:8080)
|
v
MySQL running on local machine (localhost:3306)
---
When running with Docker Compose:

Browser
|
v
Frontend Container (React)
|
v
Backend Container (Spring Boot)
|
v
MySQL Container
---

Doctor APIs
GET /doctors → get all doctors
POST /doctors → add doctor
DELETE /doctors/{id} → delete doctor
Patient APIs
GET /patients → get all patients
POST /patients → add patient
DELETE /patients/{id} → delete patient
Appointment APIs
GET /appointments → get all appointments
POST /appointments → create appointment
PUT /appointments/cancel/{id} → cancel appointment
DELETE /appointments/{id} → delete appointment

---

9. Running the Application Locally
   Backend

Make sure MySQL is running and database clinic exists.

Run backend:

mvn spring-boot:run

Backend URL:

http://localhost:8080
Frontend

Go to frontend folder:

cd frontend
npm start

Frontend URL:

http://localhost:3000
10. Running the Application with Docker
    Build backend jar
    mvn clean package
    Start all services
    docker compose up --build
    Services
    Frontend → http://localhost:3000
    Backend → http://localhost:8080
    MySQL → port 3307