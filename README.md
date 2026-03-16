# JWT Authentication API

## Description

This project is a **User Authentication and Authorization API** built with **Node.js, Express.js, and MongoDB**.
It uses **JWT (JSON Web Token)** for secure authentication and follows the **MVC architecture**.

## Tech Stack

- Node.js
- Express.js
- MongoDB (Mongoose)
- JWT (jsonwebtoken)
- bcryptjs
- Postman

## Features

- User Registration
- User Login
- Password Hashing
- JWT Token Generation
- Protected Routes using Bearer Token
- MVC Project Structure

## Project Structure

```
auth-app
│
├── config
├── controllers
├── middleware
├── models
├── routes
├── app.js
├── package.json
└── README.md
```

## Installation

Install dependencies:

```
npm install
```

Run the server:

```
npm run dev
```

Server runs on:

```
http://localhost:5000
```

## API Endpoints

### Register User

POST `/api/auth/register`

```
{
 "username": "john",
 "email": "john@gmail.com",
 "password": "123456"
}
```

### Login User

POST `/api/auth/login`

```
{
 "email": "john@gmail.com",
 "password": "123456"
}
```

Returns a **JWT Token**.

### Get User Profile (Protected)

GET `/api/auth/profile`

Header:

```
Authorization: Bearer TOKEN
```

## Testing

All APIs are tested using **Postman**.

## Author

Backend project using Node.js, Express, and MongoDB.
