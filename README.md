# Login Registration System

![Project Demo](https://user-images.githubusercontent.com/74038190/212748842-9fcbad5b-6173-4175-8a61-521f3dbb7514.gif)


This project is a user registration and login system implemented using React for the front-end and Spring Boot for the backend.

## 🚀 Technologies

- **Frontend**: React, React Router, Axios
- **Backend**: Spring Boot, Spring Data JPA, Lombok
- **Data base**: H2

## 📂 Project structure

### Backend (Spring Boot)

- `controller/MyUsersController.java` – a controller for processing user requests
- `entity/MyUsers.java` – userEnity
- `repository/MyUsersRepository.java` – interface for working with databases
- `requestResponse/LoginRequest.java` – the object of the login request
- `service/MyUsersService.java` – service for processing authorization logic

### Frontend (React)
- `src/components/login/Login.jsx` – the login page component
- `src/components/register/Register.jsx` – component of the registration page
- `src/App.js` – application routing

## 🔧 Installation and launch

### Backend (Spring Boot)
1. Make sure that you have **Java 17+** and **Maven** installed.
2. Clone the repository:
   ```sh
   git clone https://github.com/tteemma/ReactAuth.git
   cd ReactAuth
   ```
3. Launch the backend application:
   ```sh
   mvn spring-boot:run
   ```

### Frontend (React)
1. Go to the folder `frontend`:
   ```sh
   cd frontend
   ```
2. Install the dependencies:
   ```sh
   npm install
   ```
3. Launch the React application:
   ```sh
   npm run dev
   ```

## 🌍 API Endpoints

- **`POST /api/v1/users/addUser`** – Register new user
- **`POST /api/v1/users/loginUser`** – Login user

## 📌 Notes
- By default, the frontend runs on **http://localhost:5173 **.
- The backend works on **http://localhost:8080 **.
- Don't forget to configure CORS if you use it in production.

