# React & Spring Boot Authentication System

This is a simple user authentication system built with **React** for the frontend and **Spring Boot** for the backend. The application allows users to **register** and **log in** using their email and password.

## Features
- User registration
- User login authentication
- REST API with Spring Boot
- Frontend built with React and Axios for API requests
- Uses JPA for database management

## Technologies Used
### Backend:
- **Spring Boot**
- **Spring Data JPA**
- **H2 / MySQL Database**
- **Spring Web**
- **Lombok**

### Frontend:
- **React**
- **React Router**
- **Axios**
- **CSS for styling**

## Installation & Setup

### 1. Clone the Repository:
```sh
git clone https://github.com/your-username/your-repository.git
cd your-repository
2. Backend Setup (Spring Boot)
Prerequisites:
Java 17+
Maven or Gradle
Steps:
Open the backend project in your preferred IDE.
Configure database connection in application.properties (or use H2 for in-memory testing).
Run the Spring Boot application:
sh
Копировать
Редактировать
mvn spring-boot:run
or if using Gradle:
sh
Копировать
Редактировать
./gradlew bootRun
The backend will run on http://localhost:8080.
3. Frontend Setup (React)
Prerequisites:
Node.js & npm installed
Steps:
Navigate to the React frontend folder:
sh
Копировать
Редактировать
cd frontend
Install dependencies:
sh
Копировать
Редактировать
npm install
Start the React app:
sh
Копировать
Редактировать
npm run dev
The frontend will run on http://localhost:5173.
API Endpoints
Method	Endpoint	Description
POST	/api/v1/users/addUser	Register a new user
POST	/api/v1/users/loginUser	Login authentication
Project Structure
css
Копировать
Редактировать
/backend
  ├── src/main/java/artem/mironenko/loginregistrationreact
  │   ├── controller/MyUsersController.java
  │   ├── entity/MyUsers.java
  │   ├── repository/MyUsersRepository.java
  │   ├── requestResponse/LoginRequest.java
  │   ├── service/MyUsersService.java
  │   ├── LoginRegistrationReactApplication.java
  │
/frontend
  ├── src
  │   ├── components
  │   │   ├── login/Login.jsx
  │   │   ├── register/Register.jsx
  │   ├── App.jsx
  │   ├── main.jsx
  │
  ├── public
  ├── package.json
  ├── vite.config.js
Future Improvements
Implement JWT-based authentication
Add password encryption (BCrypt)
Improve UI/UX
