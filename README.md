# 🚀 Subscription Tracker - Expense Tracker Backend  

A backend service built with **Node.js, Express, and MongoDB** that allows users to **create an account, manage subscriptions, and receive email notifications before subscriptions expire**. This project enhances security with **ArCject**, manages workflows using **Upstash**, and ensures authentication via **JWT and bcrypt**.

![GitHub Repo Stars](https://img.shields.io/github/stars/v9dev/subscription-tracker?style=social)  
![GitHub forks](https://img.shields.io/github/forks/v9dev/subscription-tracker?style=social)  

---

## 📌 Table of Contents  
- [Features](#features)  
- [Tech Stack](#tech-stack)  
- [Installation](#installation)  
- [API Endpoints](#api-endpoints)  
- [Security](#security)  
- [Workflow](#workflow)  
- [Contributing](#contributing)  
- [License](#license)  
- [Contact](#contact)  

---

## ✨ Features  
✅ **User Authentication** – Sign up & login using JWT and bcrypt  
✅ **Subscription Management** – Add, edit, and track subscriptions  
✅ **Automated Expiry Alerts** – Sends email reminders before subscription expires  
✅ **Security with ArCject** – Ensures strong data protection  
✅ **Workflow Automation with Upstash** – Efficient background job handling  
✅ **MongoDB Models & Schema** – Organized data management with Mongoose  

---

## 🛠 Tech Stack  
![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Nodemon](https://img.shields.io/badge/NODEMON-%23323330.svg?style=for-the-badge&logo=nodemon&logoColor=%BBDEAD)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens) ![NPM](https://img.shields.io/badge/NPM-%23CB3837.svg?style=for-the-badge&logo=npm&logoColor=white)

| **Category** | **Technology** |  
|-------------|---------------|  
| Backend | Node.js, Express.js |  
| Database | MongoDB (Mongoose ORM) |  
| Authentication | JWT, bcrypt |  
| Security | ArCject |  
| Workflow Automation | Upstash |  
| Email Notifications | Nodemailer (or similar) |  

---

## 🛠 Installation  
### Prerequisites  
- Install **Node.js**: [Download here](https://nodejs.org/en/download/)  
- Create account on **MongoDB**: [Link](https://www.mongodb.com/cloud/atlas/register)  

### Steps  
1. **Clone the repository**  
   ```sh
   git clone https://github.com/v9dev/subscription-tracker.git
   cd subscription-tracker
   ```

2. **Install dependencies**  
   ```sh
   npm install
   ```

3. **Set up environment variables**  
   Create a `.env` file in the root directory and add the following:  
   ```sh
    # Server
    PORT=5500

    ERVER_URL = "http://localhost:5500"
    NODE_ENV=development

    # Database
    DB_URI=Your Mongo DB URL


    # JWT auth 

    JWT_SECRET = "YOUR JWT SECRET"
    JWT_EXPIRES_IN = "1d"


    # ARCJET
    ARCJET_KEY= "arcject_key"
    ARCJET_ENV="development"

    # UPSTASH

    QSTASH_URL = "http://127.0.0.1:8080"
    QSTASH_TOKEN=your_qstash_token

    # NODEMAILER
    EMAIL_PASSWORD= "Your Email Password" #Go to Manage Your Google account and search for the App Password and Create New App
   ```

4. **Start the server**  
   ```sh
   npm start
   ```
   The server will run on `http://localhost:5000`.

---

## 📡 API Endpoints  
### 🔑 Authentication  
| Method | Endpoint | Description |  
|--------|---------|-------------|  
| POST | `/api/auth/signup` | Register a new user |  
| POST | `/api/auth/login` | Login and get JWT token |  

### 📅 Subscription Management  
| Method | Endpoint | Description |  
|--------|---------|-------------|  
| POST | `/api/subscriptions` | Add a new subscription |  
| GET | `/api/subscriptions` | Get all subscriptions |  
| GET | `/api/subscriptions/:id` | Get subscription by ID |  
| PUT | `/api/subscriptions/:id` | Update a subscription |  
| DELETE | `/api/subscriptions/:id` | Remove a subscription |  
  

---

## 🔒 Security  
- **JWT Authentication** – Secure API endpoints with JSON Web Tokens  
- **Bcrypt Hashing** – Encrypts user passwords  
- **ArCject Security** – Additional security layer  
- **Upstash Workflow Management** – Secure workflow automation  

---

## 🔄 Workflow  
1. **User registers & logs in**  
2. **Adds subscriptions (e.g., Netflix, Spotify, etc.)**  
3. **System tracks subscription expiry dates**  
4. **Email reminders sent before expiry**  
5. **User can update or remove subscriptions**  

---

## 🤝 Contributing  
We welcome contributions! Follow these steps:  
1. **Fork** the repository  
2. **Create a feature branch** (`git checkout -b feature-xyz`)  
3. **Commit your changes** (`git commit -m "Add feature xyz"`)  
4. **Push to the branch** (`git push origin feature-xyz`)  
5. **Open a Pull Request**  

---


## 📞 Contact  
📧 Email: thisjpsingh@gmail.com 
📘 LinkedIn: [Jitendra Pratap Singh](https://linkedin.com/in/iamjpsingh)  
