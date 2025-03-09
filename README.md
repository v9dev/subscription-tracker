# Subscription Tracker

This is Subscription tracker project that allow to create user and create a subscription and tract them by sending them a email when the subscriptionn getting expering.

We are using express.js for the backend monogo db for database mongooes for schema arcject for security and qstach for the workflow.

You have to setup these things

Fist create a monogo db alter use the DB URI
Second create arcjet and add key
Jwt
Qstacsh

**You can just clone this repo and setup all the config then can run**

First 

```
npm install
npm run dev
```

**Before Goinng to test you have to create .env.development.local and .env.production.local file with these config**

```#Server
PORT=5500

SERVER_URL = "http://localhost:5500"
NODE_ENV=development

# Database
DB_URI=mongodb+srv://username:password@project.zgqch.mongodb.net/?retryWrites=true&w=majority&appName=projectname


#JWT auth 

JWT_SECRET = "yourjwtsecret"
JWT_EXPIRES_IN = "1d"


# ARCJET
ARCJET_KEY= "yourarcjeckey"
ARCJET_ENV="development"

# UPSTASH

QSTASH_URL = "http://127.0.0.1:8080"
QSTASH_TOKEN=yourqstashtoken

# NODEMAILER
EMAIL_PASSWORD= "Your Pass Word"
```