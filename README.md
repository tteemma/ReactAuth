# Login Registration System

Этот проект представляет собой систему регистрации и входа пользователей, реализованную с использованием React для фронтенда и Spring Boot для бэкенда.

## 🚀 Технологии

- **Frontend**: React, React Router, Axios
- **Backend**: Spring Boot, Spring Data JPA, Lombok
- **База данных**: H2 (по умолчанию) или любая другая реляционная БД

## 📂 Структура проекта

### Backend (Spring Boot)
- `controller/MyUsersController.java` – контроллер для обработки запросов пользователей
- `entity/MyUsers.java` – сущность пользователя
- `repository/MyUsersRepository.java` – интерфейс для работы с БД
- `requestResponse/LoginRequest.java` – объект запроса для входа
- `service/MyUsersService.java` – сервис для обработки логики авторизации
- `LoginRegistrationReactApplication.java` – точка входа Spring Boot приложения

### Frontend (React)
- `src/components/login/Login.jsx` – компонент страницы входа
- `src/components/register/Register.jsx` – компонент страницы регистрации
- `src/App.js` – роутинг приложения

## 🔧 Установка и запуск

### Backend (Spring Boot)
1. Убедитесь, что у вас установлен **Java 17+** и **Maven**.
2. Склонируйте репозиторий:
   ```sh
   git clone https://github.com/tteemma/ReactAuth.git
   cd ReactAuth
   ```
3. Запустите бэкенд-приложение:
   ```sh
   mvn spring-boot:run
   ```

### Frontend (React)
1. Перейдите в папку `frontend`:
   ```sh
   cd frontend
   ```
2. Установите зависимости:
   ```sh
   npm install
   ```
3. Запустите React-приложение:
   ```sh
   npm run dev
   ```

## 🌍 API Эндпоинты

- **`POST /api/v1/users/addUser`** – Регистрация нового пользователя
- **`POST /api/v1/users/loginUser`** – Вход пользователя

## 📌 Заметки
- По умолчанию, фронтенд работает на **http://localhost:5173**.
- Бэкенд работает на **http://localhost:8080**.
- Не забудьте настроить CORS, если используете в продакшене.

## 📜 Лицензия
Этот проект распространяется под лицензией MIT.

