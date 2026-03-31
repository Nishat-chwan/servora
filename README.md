# SerVora – A Local Service Booking System with AI Integration

## Team Members
| Name | Email |
|------|------|
| MOHSINA | mohsina.cse.20220204027@aust.edu |
| ANJUM | anjum.cse.20220204044@aust.edu |
| NISHAT | nishat.cse.20220204049@aust.edu |
| RIA | ria.cse.20220204050@aust.edu |

---

## Project Live Link
[**SerVora Live**](https://servorax.vercel.app)

---

## Table of Contents
- [Project Description](#project-description)
- [Workflow Overview](#workflow-overview)
- [Main Features](#main-features)
- [Technologies Used](#technologies-used)
- [System Architecture](#system-architecture)
- [Setup Guidelines](#setup-guidelines)
- [Running the Application](#running-the-application)
- [Deployment Status & Tests](#deployment-status--tests)
- [Contribution Table](#contribution-table)
- [Screenshots](#screenshots)
- [Limitations / Known Issues](#limitations--known-issues)

---

## Project Description
SerVora is a web-based platform that connects customers with trusted local service providers (electricians, tutors, plumbers, etc.).  
Users can search, book, and rate services.  
The system uses **AI-driven recommendations** to suggest the most relevant providers based on location, past behavior, ratings, and service category.

---

## Workflow Overview
1. A customer signs up and logs in.  
2. Browses or searches for services by category, location, and availability.  
3. AI module ranks suitable providers for the requested service.  
4. Customer books an appointment; provider accepts or rejects.  
5. After service delivery, customer submits reviews and ratings.  
6. Admin approves providers, manages users/services/payments, and views analytics.

---

## Main Features
- User registration with roles: **Customer**, **Service Provider**, **Admin**  
- Service browsing/filtering by category, location, and availability  
- Provider verification via uploaded documents  
- Booking system: create, update, cancel appointments  
- Secure payment integration (**COD**)  
- Reviews & ratings with admin moderation  
- AI recommendations for best-fit providers  
- Admin dashboard for managing services, users, bookings, and payments

---

## Technologies Used
| Layer        | Tools / Frameworks                |
|--------------|-----------------------------------|
| **Backend**  | Laravel 11                         |
| **Frontend** | React.js                           |
| **Database** | MySQL                               |
| **Auth**     | JWT Token         |
| **AI**       | Gemini Ai                |
| **Roles**    | Spatie Laravel-Permission          |

---

## System Architecture
- **Frontend (React.js)** interacts with the **Laravel backend** via RESTful APIs.  
- For AI-based recommendations, the backend forwards user/request data (history, location, service type, provider ratings/availability) to a **Flask-based AI service**.  
- Laravel handles authentication, role & permissions, payments, document verification, and booking workflows.  
- **MySQL** stores users, services, bookings, reviews, provider documents, and more.

---

## Setup Guidelines
```bash
# Clone or download the project repo (if available)

# Backend setup
cd backend
composer install
cp .env.example .env
# Set environment variables: DB connection, SSLCommerz keys, AI API endpoint, etc.

# Frontend setup
cd frontend
npm install
# Configure environment variables (API base URL, map API keys, etc.)
npm start
Running the Application

Start the Laravel backend server.

Start the Flask AI service.

Start the React frontend.

Visit SerVora Live in a browser to interact.


| Component | Deployed? | Dockerized? | Unit Tests? | AI Feature? |
| --------- | --------- | ----------- | ----------- | ----------- |
| Backend   | Yes       | Yes          | No          | Yes         |
| Frontend  | Yes       | Yes          | No          | Yes         |

| Member                | Issues Solved | WakaTime Hours | Percent Contribution |
| --------------------- | ------------- | ---------------- | -------------------- |
| S. M. Sadnan Saher    | 5             | [![wakatime](https://wakatime.com/badge/user/7bff677b-9b77-497c-ba7d-29ffc0f02148/project/bc90ae10-b528-47c5-8c41-a9990245bcad.svg)](https://wakatime.com/badge/user/7bff677b-9b77-497c-ba7d-29ffc0f02148/project/bc90ae10-b528-47c5-8c41-a9990245bcad)               | 21%                  |
| Md. Mehedi Hasan Rafi |  8            | [![wakatime](https://wakatime.com/badge/user/1cb697c9-d16a-4c4d-a6e2-af85e61b283b/project/599c75c7-b4a0-4d15-baa6-26e2c85b34bb.svg)](https://wakatime.com/badge/user/1cb697c9-d16a-4c4d-a6e2-af85e61b283b/project/599c75c7-b4a0-4d15-baa6-26e2c85b34bb)               | 34%                  |
| Mahdi Khan Chowdhury  | 10            | [![wakatime](https://wakatime.com/badge/user/9d96a11b-73d5-4a6c-9587-a9efa87ef402/project/f8668182-0ff6-47f9-a237-37c295166e68.svg)](https://wakatime.com/badge/user/9d96a11b-73d5-4a6c-9587-a9efa87ef402/project/f8668182-0ff6-47f9-a237-37c295166e68)               | 41%                  |
| Fatah Uddin           | 1             | [![wakatime](https://wakatime.com/badge/user/b160ce15-9c18-43ac-8c74-1af63808bc1f/project/dc94b2f4-4f1e-4e60-87d3-e0ca6b711ef1.svg)](https://wakatime.com/badge/user/b160ce15-9c18-43ac-8c74-1af63808bc1f/project/dc94b2f4-4f1e-4e60-87d3-e0ca6b711ef1)               | 4%                   |

Screenshots
<img width="2230" height="1303" alt="Screenshot 1" src="https://github.com/user-attachments/assets/a28c0dc7-6928-4c50-a3de-c176532af9aa" /> <img width="2226" height="1301" alt="Screenshot 2" src="https://github.com/user-attachments/assets/d8069ec3-cb75-4ce1-b273-61978abbf50a" /> <img width="2231" height="1302" alt="Screenshot 3" src="https://github.com/user-attachments/assets/a1f7fafe-25cb-4378-b17d-b12f08d3a251" /> <img width="2227" height="1299" alt="Screenshot 4" src="https://github.com/user-attachments/assets/190857bc-df1e-4c16-83d1-e512f113f9c6" /> <img width="2253" height="1297" alt="Screenshot 5" src="https://github.com/user-attachments/assets/26d7e972-c674-435b-8faf-a7638936e148" /> <img width="2251" height="1296" alt="Screenshot 6" src="https://github.com/user-attachments/assets/23ef0dd5-0347-48da-8552-9d287c5afd95" /> <img width="2231" height="1299" alt="Screenshot 7" src="https://github.com/user-attachments/assets/83d3754d-be74-4c22-b857-a3117d888e6c" /> <img width="2229" height="1298" alt="Screenshot 8" src="https://github.com/user-attachments/assets/91d33d5c-566d-416b-a3eb-458624b6758b" /> <img width="2232" height="1277" alt="Screenshot 9" src="https://github.com/user-attachments/assets/71e9b41c-b227-4e66-9120-fe9dfc014826" /> <img width="2237" height="1298" alt="Screenshot 10" src="https://github.com/user-attachments/assets/16d96571-58cb-4aa5-b5ac-bd62bbbf2f7b" /> <img width="2231" height="1302" alt="Screenshot 11" src="https://github.com/user-attachments/assets/6567f0a8-539f-4b94-987c-e8b8ceb9abdc" />


Limitations / Known Issues

Some AI recommendation refinements/edge-cases might not be fully optimized.
No unit tests currently.
Missing certain features such as email/SMS verification latenc