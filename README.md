# MERN Starter

A full-stack web application built with the MERN stack (MongoDB, Express, React, Node.js), featuring user authentication, profiles, and posts.

**Live Demo:** https://mern-starter-uk9f.onrender.com

> Note: This app is hosted on Render's free plan. If it has been inactive, the first load may take around 50 seconds while the server wakes up.

## Features

- User registration and login with JWT authentication
- Google login (OAuth)
- Email notifications and account activation
- SMS verification (Twilio)
- User profiles
- Create and manage posts
- Contact form
- File uploads

## Tech Stack

- **Frontend:** React, Redux
- **Backend:** Node.js, Express
- **Database:** MongoDB (Atlas)
- **Authentication:** JSON Web Tokens, Google OAuth
- **Hosting:** Render

## Project Structure

client/ React frontend
config/ Database configuration
email/ Email templates and sending
middleware/ Authentication middleware
models/ Mongoose models (User, Profile, Post, Contact)
routes/api/ API routes (auth, users, profile, posts, contacts, uploads)
sms/ SMS sending (Twilio)
server.js Express server entry point


## Getting Started (Local)

1. Clone the repository:

git clone https://github.com/tharimakeya-dev/mern-starter.git
cd mern-starter


2. Install dependencies:

npm install
npm install --prefix client


3. Create `config/default.json` with your own values:
```json
   {
     "mongoURI": "your-mongodb-connection-string",
     "jwtSecret": "your-jwt-secret",
     "googleClientID": "your-google-client-id"
   }
```

4. Set the environment variables used by the app: `ADMIN_EMAIL`, `FRONTEND_URL`, `GMAIL_USER`, `GMAIL_PASSWORD`, `TWILIO_ACCOUNT_SID`, `TWILIO_AUTH_TOKEN`, `TWILIO_PHONE_NUMBER`.

5. Run the app:

npm start


## Deployment

Deployed on Render. Secrets are stored in Render's Secret Files and Environment Variables, not in the repository.

## Author

[tharimakeya-dev](https://github.com/tharimakeya-dev)

# Mern-starter
Live Demo: https://mern-starter-uk9f.onrender.com
