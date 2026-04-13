# Online Banking System

## Overview

This project is a simplified Online Banking System developed as part of a hackathon.
It allows users to create accounts, check balances, and perform secure fund transfers.

The system is designed using a 3-tier architecture with a focus on security, scalability, and clean design.

---

## Features

### User Features

* User Registration and Login
* Account Creation
* Check Account Balance
* Transfer Funds
* View Transaction History

### Security Features

* JWT-based Authentication
* Password Hashing (SHA-256)
* OTP Generation
* Role-based Access Control
* Basic Fraud Detection

### Admin Features

* View Users
* Monitor Transactions

---

## System Architecture

The system follows a 3-tier architecture:

* Frontend: React (UI)
* Backend: FastAPI (REST APIs)
* Database: PostgreSQL (Relational DB)

### Flow

1. User interacts with UI
2. UI sends request to backend APIs
3. Backend processes business logic
4. Data is stored or retrieved from database
5. Response is sent back to user

---

## Technology Stack

| Layer    | Technology | Reason                                      |
| -------- | ---------- | ------------------------------------------- |
| Frontend | React      | Dynamic UI and component-based structure    |
| Backend  | FastAPI    | High performance and easy API development   |
| Database | PostgreSQL | Strong consistency and relational integrity |
| Auth     | JWT        | Secure and stateless authentication         |

---

## Project Structure

```
banking-system/
│
├── backend/
│   └── app/
│       ├── models/
│       ├── routes/
│       ├── services/
│       ├── utils/
│       ├── dependencies/
│       ├── constants/
│
├── frontend/
│   └── src/
│       ├── pages/
│       ├── components/
│       ├── services/
│       ├── context/
│
└── README.md
```

---

## Key Modules (My Contribution)

* JWT Token Handling (jwt_handler.py)
* Password Hashing (password.py)
* OTP Generation (otp.py)
* Fraud Detection (fraud_detection.py)
* Authentication Dependency
* Role-based Access Control

---

## Core Logic

### Fund Transfer

* Validate sufficient balance
* Deduct amount from sender
* Add amount to receiver
* Store transaction details

### Security

* Passwords stored in hashed format
* JWT tokens used for authentication
* Role-based access restrictions

---

## Edge Cases Handled

* Insufficient Balance
* Invalid Token
* Unauthorized Access
* High-value Transaction Detection

---

## Future Enhancements

* Advanced Fraud Detection (ML-based)
* Real-time Notifications
* Multi-factor Authentication
* UI Improvements

---

## Team Collaboration

This project was developed as a team effort, with clear separation of responsibilities across backend, frontend, and security modules.

---

## Conclusion

This system demonstrates a scalable and secure approach to building a digital banking platform with core functionalities and clean architecture.

