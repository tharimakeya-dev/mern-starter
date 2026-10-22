# MERN Starter

A full-stack web application built with the MERN stack (MongoDB, Express, React, Node.js), featuring user authentication, profiles, and posts.

**Live Demo:** mern-starter-uk9f.onrender.com


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

```
mern-starter/
├── client/          # React frontend
├── config/          # Database configuration
├── email/           # Email templates and sending
├── middleware/      # Authentication middleware
├── models/          # Mongoose models (User, Profile, Post, Contact)
├── routes/api/      # API routes (auth, users, profile, posts, contacts, uploads)
├── sms/             # SMS sending (Twilio)
└── server.js        # Express server entry point
```

## Getting Started (Local)

### 1. Clone the repository

```bash
git clone https://github.com/tharimakeya-dev/mern-starter.git
cd mern-starter
```

### 2. Install dependencies

```bash
npm install
npm install --prefix client
```

### 3. Create `config/default.json` with your own values

```json
{
  "mongoURI": "your-mongodb-connection-string",
  "jwtSecret": "your-jwt-secret",
  "googleClientID": "your-google-client-id"
}
```

> **Note:** Never commit real secrets. Add `config/default.json` and `.env` to your `.gitignore`.

### 4. Set the environment variables

The app uses the following environment variables. Set them in your terminal or in a `.env` file in the project root:

```env
ADMIN_EMAIL=your-admin-email
FRONTEND_URL=http://localhost:3000
GMAIL_USER=your-gmail-address
GMAIL_PASSWORD=your-gmail-app-password
TWILIO_ACCOUNT_SID=your-twilio-account-sid
TWILIO_AUTH_TOKEN=your-twilio-auth-token
TWILIO_PHONE_NUMBER=your-twilio-phone-number
```

### 5. Run the app

```bash
npm start
```

## Deployment

Deployed on Render. Secrets are stored in Render's Secret Files and Environment Variables, not in the repository.

## Author

[tharimakeya-dev](https://github.com/tharimakeya-dev)
