# Subscription Tracker

**This is a subscription tracker Api Before Goinng to test you have to create .env.development.local and .env.production.local file with these config**

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