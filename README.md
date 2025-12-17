# FitTrack Demo

## Project Overview

FitTrack Demo is a simple fitness tracking web application built as a course demo project. It demonstrates user authentication, workout tracking, and workout history storage using **Firebase**.

The project focuses on:

* Frontend integration with Firebase
* Email/Password authentication
* Storing and retrieving user-specific data from Firestore
* Preparing a complete deliverable suitable for a live demo or recorded presentation

---

## Features

*  User Registration & Login (Firebase Authentication)
*  Add Workout Records (type, duration, notes)
*  View Workout History per User
*  Protected Pages (only accessible after login)
*  Cloud Firestore for persistent data storage
*  Clean, modern UI (HTML + CSS)

---

## Project Architecture

* **Frontend:** HTML, CSS, JavaScript
* **Backend (BaaS):** Firebase

  * Authentication (Email/Password)
  * Cloud Firestore (NoSQL Database)

Each authenticated user has their own workout data stored securely in Firestore.

---

## Project Structure

```
FitTrack-Demo/
│
├── index.html          # Landing page
├── login.html          # Login & Register page
├── dashboard.html      # User dashboard
├── tracking.html       # Add workouts
├── history.html        # View workout history
│
├── firebase.js         # Firebase configuration
├── auth.js             # Authentication logic
├── tracking.js         # Firestore write logic
├── history.js          # Firestore read logic
│
├── styles.css          # Shared styling
├── README.md           # Project documentation
└── .gitignore
```

---

## How to Run Locally

1. Clone the repository:

```bash
git clone https://github.com/Maramnagy/FitTrack-Demo
```

2. Open the project folder:

```bash
cd FitTrack-Demo
```

3. Open `index.html` using Live Server or directly in a browser

4. Make sure Firebase services are enabled:

* Authentication → Email/Password
* Cloud Firestore → Test mode

---

## Demo Instructions

Suggested demo flow:

1. Open the landing page
2. Register a new user
3. Login with the created account
4. Add a workout
5. Open History page and show stored data

---

## Known Limitations

* No password reset functionality
* Basic UI (no framework)
* Firestore rules are in test mode (for demo only)

---

## Future Improvements

* Add charts and analytics
* Improve UI with a framework (React / Vue)
* Add profile page
* Implement Firestore security rules

---

## Author

Maram Mohamed


