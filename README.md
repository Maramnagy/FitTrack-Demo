# FitTrack Demo

## Project Overview

FitTrack Demo is a simple fitness tracking web application built as a course demo project. It demonstrates user authentication, workout tracking, and workout history storage using **Firebase**.

The project focuses on:

* Frontend integration with Firebase
* Email/Password authentication
* Storing and retrieving user-specific data from Firestore
* Preparing a complete deliverable suitable for a live demo or recorded presentation
* Integrates Firebase Cloud Firestore to store workout data persistently from the frontend
---

## Features

*  User Registration & Login (Firebase Authentication)
*  Add Workout Records (name, duration, calories)
*  View Workout History per User
*  Protected Pages (only accessible after login)
*  Cloud Firestore for persistent data storage
*  Frontend : Clean, modern UI (HTML + CSS3 + JavaScript (ES Modules) + Firebase SDK (Web v10))
*  Backend : Firebase Authentication, Firebase Cloud Firestore, Firebase Hosting
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
├── login.html          # User authentication (Firebase Auth)
│                        (Auth logic implemented directly inside the page)
├── tracking.html       # Add workout (Firestore write)
│                        (Firestore write logic implemented inside the page)
├── history.html        # View workout history (Firestore read)
│                        (Firestore read logic implemented inside the page)
│
├── firebase.js         # Firebase configuration (Auth + Firestore)
├── styles.css          # Shared styling
│
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
cd FitTrack-Project
```

3. Install Firebase CLI and log in:
```bash
npm install -g firebase-tools
firebase login
```
4. Deploy the application to Firebase Hosting:
```bash
firebase deploy
```
5. Open the deployed application using the generated hosting URL:
https://fittrack-demo-51bb1.web.app

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


