# WEB AUTHENTICATION

A Node.js web application that lets users anonymously share their secrets. Built with Express, MongoDB, and Passport.js, it demonstrates modern bcrypt authentication techniques including local login and Google OAuth.

# 📚 Section Coverage (From Course)

This app was developed as part of **Section 35: Authentication and Security** of a web development course. The section includes:
- Email/password registration with encryption
- Password salting and hashing
- Session and cookie management
- Using environment variables for security
- Google OAuth integration

# 🚀 Features

- Register and login with email and password
- Passwords are encrypted and salted with bcrypt
- Option to login using Google OAuth 2.0
- Secrets submitted anonymously and displayed to all users
- Sessions and cookies handled securely
- Sensitive credentials managed with environment variables

# 🛠️ Tech Stack

- **Frontend**: HTML, EJS, Bootstrap
- **Backend**: Node.js, Express
- **Database**: MongoDB (via Mongoose)
- **Authentication**: Passport.js (Local Strategy & Google OAuth 2.0)
- **Encryption**: bcrypt
- **Session Management**: express-session
- **Environment Variables**: dotenv

# 🔧 Installation

1. Clone the repository:
   i. git clone https://github.com/your-username/secrets-app.git
   ii. cd secrets-app

2. Install dependencies:
  npm install

3. Create a .env file in the root directory:

GOOGLE_CLIENT_ID=our_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
SESSION_SECRET=YOUR_SECRET_WORD
PG_USER=YOUR_DATABSE
PG_HOST="localhost"
PG_DATABASE=YOUR_DATABSE_NAME
PG_PASSWORD=YOUR_DATABASE_PASSWORD
PG_PORT=DATABAE_PORT

4. Run the server:
  nodemon index.js

5. Open your browser and navigate to:
   http://localhost:3000

# 🌐 Routes
Route	        Description
/	Home        page
/register	    Register a new user
/login	      Login existing user
/submit	      Submit an anonymous secret
/secrets	    View all shared secrets
/logout	      Logout and end user session
/auth/google	Google OAuth sign-in

# 🔐 Security Measures
Passwords are hashed and salted using bcrypt

Sessions are secured using express-session

API keys and secrets stored in environment variables

OAuth 2.0 login via Google

# 🧠 What I Learned
Handling user authentication securely

Implementing OAuth 2.0 in Node.js

Managing environment variables

Working with cookies and sessions

Using Passport.js with multiple strategies


# 📄 License
This project is open source and available under the MIT License.
  

   
   
