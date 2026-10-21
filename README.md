# JWT-authentication-project
Implemented JWT Authentication in Django REST Framework using SimpleJWT, including user login, access and refresh tokens, and token-based API authentication.
# JWT Authentication with Django REST Framework

## 📌 About the Project

This project demonstrates the implementation of **JWT (JSON Web Token) Authentication** using Django REST Framework and SimpleJWT.

It allows users to authenticate themselves and receive access and refresh tokens for token-based API authentication. The project focuses on understanding how authentication works in REST APIs.

## 🚀 Features

- User login and authentication
- JWT access token generation
- JWT refresh token generation
- Token-based API authentication
- User information and role handling (if implemented)
- Django REST Framework integration

## 🛠️ Technologies Used

- Python
- Django
- Django REST Framework
- SimpleJWT
- SQLite / MySQL (depending on your database configuration)

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Navigate to the project directory:

```bash
cd YOUR_PROJECT_DIRECTORY
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install django djangorestframework djangorestframework-simplejwt
```

If your project has a `requirements.txt` file, use:

```bash
pip install -r requirements.txt
```

### 4. Apply Migrations

```bash
python manage.py migrate
```

### 5. Run the Development Server

```bash
python manage.py runserver
```

The development server will be available at:

`http://127.0.0.1:8000/`

## 🔐 How JWT Authentication Works

1. The user sends login credentials to the authentication endpoint.
2. The server verifies the credentials.
3. If the credentials are valid, the server generates an access token and a refresh token.
4. The client sends the access token with requests to protected endpoints.
5. When the access token expires, the refresh token can be used to obtain a new access token, if token refresh is configured.

### Authorization Header

For protected API requests, include the access token in the request headers:

```http
Authorization: Bearer YOUR_ACCESS_TOKEN
```

## 🧪 API Testing

You can test the authentication endpoints using **Postman**.

Example login request:

```http
POST /your-login-endpoint/
Content-Type: application/json
```

Example request body:

```json
{
    "username": "your_username",
    "password": "your_password"
}
```

The exact endpoint and request fields depend on your Django project configuration.

## 📚 Learning Objectives

Through this project, I practiced:

- Understanding JWT-based authentication
- Generating access and refresh tokens
- Working with Django REST Framework
- Understanding HTTP request headers
- Using Bearer tokens for API authentication
- Testing API endpoints with Postman

## 👨‍💻 Author

**Muhammad Qasim**

GitHub: [mr-qasim1](https://github.com/mr-qasim1)

LinkedIn: [Syed Qasim](https://www.linkedin.com/in/syed-qasim-6925022a8/)

---

*This project was developed as part of my hands-on learning journey in Django REST Framework and backend development.*
