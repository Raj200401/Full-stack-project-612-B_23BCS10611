# Grievance Portal

## Project Description
The *Grievance Portal* is a web-based complaint management system that allows users to submit grievances and track their status. Administrators can view all submitted complaints, update their status, and resolve them efficiently. The platform ensures clear communication between users and administrators.

## Features
- User login and authentication  
- Submit new grievances  
- Track grievance status  
- Admin dashboard to manage all complaints  
- Secure REST API backend  
- Clean and responsive user interface  

## How the Project Works
1. **Frontend (React App)**  
   - Provides the user interface for login, registering complaints, and viewing status.  
   - Runs on **http://localhost:3000**

2. **Backend (Spring Boot)**  
   - Handles authentication, database operations, and complaint processing.  
   - Runs on **http://localhost:8081**  
   - Uses an in-memory H2 database for demonstration.

3. **Workflow**  
   - User logs in → submits a grievance → backend stores the data → admin views & resolves the issue → user sees updated status.


## How to Run the Project

### Backend + Frontend Setup (All Commands Together)

```bash
# 1. Start Backend
cd backend/grievance-backend
.\mvnw.cmd spring-boot:run
# Backend will run at: http://localhost:8081

# 2. Start Frontend (open a new terminal)
cd grievance-portal-v2
npm install
npm start
# Frontend will run at: http://localhost:3000
