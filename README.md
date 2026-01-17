# Team Directory Application

## Overview
This is a Team Directory application that retrieves employee data from a ColdFusion REST API and displays it in a React frontend. The project demonstrates full-stack development, RESTful API communication, secure database handling, and modern React patterns.

## Tech Stack
- Frontend: React (Vite)
- Backend: ColdFusion (RESTful CFC)
- Database: SQLite
- Data Format: JSON

## Features
- Fetch employee data from a ColdFusion REST API
- Display employees in a clean, user-friendly layout
- Search employees by first or last name
- Secure database queries using cfqueryparam
- CORS enabled for frontend-backend communication

## Database
- SQLite database
- Employees table fields:
  - ID
  - FirstName
  - LastName
  - Role
- Includes sample (dummy) employee records

SQL file included:
database-setup.sql

## Backend (ColdFusion)
- REST API implemented using EmployeeAPI.cfc
- Returns employee data in JSON format
- CORS headers handled in Application.cfc
- Uses cfqueryparam for security

Sample endpoint:
/cf-backend/EmployeeAPI.cfc?method=getEmployees

## Frontend (React)
- Built using Vite
- Uses useEffect to fetch API data
- Uses useState for state management
- Displays data using reusable components
- Includes search functionality (bonus)

## Project Structure
team-directory/
- src/
  - components/
    - EmployeeCard.jsx
    - SearchBar.jsx
  - App.jsx
  - main.jsx
- database-setup.sql
- README.md

cf-backend/
- Application.cfc
- EmployeeAPI.cfc
- create-database.cfm

## Evaluation Coverage
- Clean and readable code organization
- Secure API and database access
- Proper JSON handling
- Modern React Hooks usage
- Bonus search feature implemented

## Notes
A short 2-minute video explaining the frontend and backend modules can be provided if required.

## Submission
The project can be submitted as a GitHub repository or as a ZIP file containing all source code.
