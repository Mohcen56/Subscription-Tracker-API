# Subscription Tracker API

A **production-ready Subscription Management System API** that I built to get familiar with Node.js and Express.js.

<div>
  <img src="https://img.shields.io/badge/node.js-339933?style=for-the-badge&logo=Node.js&logoColor=white" alt="node.js" />
  <img src="https://img.shields.io/badge/express.js-000000?style=for-the-badge&logo=express&logoColor=white" alt="express.js" />
  <img src="https://img.shields.io/badge/-MongoDB-13aa52?style=for-the-badge&logo=mongodb&logoColor=white" alt="mongodb" />
</div>

## 📋 Table of Contents

1. 🤖 [Introduction](#introduction)
2. ⚙️ [Tech Stack](#tech-stack)
3. 🔋 [Features](#features)
4. 🤸 [Quick Start](#quick-start)
5. 🕸️ [Snippets](#snippets)

## 🤖 Introduction

I built this project to learn and get hands-on experience with **Node.js** and **Express.js**. It's a full-featured subscription management API that handles real users, authentication, and business logic.

Through this project, I learned how to:
- Authenticate users using JWTs
- Connect to a database and create models/schemas with MongoDB & Mongoose
- Structure API architecture for scalability
- Implement middleware, error handling, and input validation
- Set up automated email reminders using workflows

## ⚙️ Tech Stack

- Node.js
- Express.js
- MongoDB

## 🔋 Features

👉 **Advanced Rate Limiting and Bot Protection**: Secured with Arcjet to protect the entire app.

👉 **Database Modeling**: Models and relationships using MongoDB & Mongoose.

👉 **JWT Authentication**: User CRUD operations and subscription management.

👉 **Global Error Handling**: Input validation and middleware integration.

👉 **Logging Mechanisms**: For better debugging and monitoring.

👉 **Email Reminders**: Automated smart email reminders with workflows using Upstash.

...and more, including clean code architecture and reusability.

## 🤸 Quick Start

Follow these steps to set up the project locally on your machine.

**Prerequisites**

Make sure you have the following installed on your machine:

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/en)
- [npm](https://www.npmjs.com/) (Node Package Manager)

**Installation**

Install the project dependencies using npm:

```bash
npm install
```

**Set Up Environment Variables**

Create a new file named `.env.local` in the root of your project and add the following content:

```env
# PORT
PORT=5500
SERVER_URL="http://localhost:5500"

# ENVIRONMENT
NODE_ENV=development

# DATABASE
DB_URI=

# JWT AUTH
JWT_SECRET=
JWT_EXPIRES_IN="1d"

# ARCJET
ARCJET_KEY=
ARCJET_ENV="development"

# UPSTASH
QSTASH_URL=http://127.0.0.1:8080
QSTASH_TOKEN=

# NODEMAILER
EMAIL_PASSWORD=
```

**Running the Project**

```bash
npm run dev
```

Open [http://localhost:5500](http://localhost:5500) in your browser or any HTTP client to test the project.

## 🕸️ Snippets

<details>
<summary><code>Sample Subscription JSON</code></summary>

```json
{
  "name": "Premium Membership",
  "price": 139.00,
  "currency": "USD",
  "frequency": "monthly",
  "category": "Entertainment",
  "startDate": "2025-01-20T00:00:00.000Z",
  "paymentMethod": "Credit Card"
}
```

</details>
