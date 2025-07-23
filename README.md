# 🚀 Chat App (MERN + Socket.IO)

A real-time chat application built with the MERN stack (MongoDB, Express, React, Node.js) and Socket.IO, featuring user authentication, notifications, profile management, and CI/CD pipelines with monitoring.

---

## 🔗 Live URLs

- **Frontend:** [https://client-chi-rosy-78.vercel.app/]
- **Backend API:** [https://chatappserver-kwaj.onrender.com]

---

## 🛠️ Features

- 🔐 User Authentication (JWT)
- 🧑 User Profiles
- 💬 Real-time messaging with Socket.IO
- 🔔 Notifications
- 📝 Edit/Delete Jobs
- 📈 Monitoring and CI/CD via GitHub Actions, Sentry, and UptimeRobot

---

## 📸 Screenshots

### ✅ CI/CD Pipeline (GitHub Actions)

**Backend Tests + Deploy**  
![Backend CI/CD](screenshot\backend.png)

**Frontend CI/CD**  
![Frontend CI/CD](screenshot\frontend.png)

---

## 🔁 Continuous Integration & Deployment

### ✅ Backend

- **Trigger:** On push to `main`
- **Steps:** Install deps → Run tests → Trigger Render deploy
- **File:** `.github/workflows/deploy.yml` in backend repo

### ✅ Frontend

- **Trigger:** On push to `main`
- **Steps:** Install deps → Build → Deploy to Vercel via GitHub integration

---

## 🔍 Monitoring & Health

### ✅ Uptime Monitoring (UptimeRobot)

- **Interval:** Every 5 minutes
- **Alerts:** Email notifications enabled


---

### ✅ Error Monitoring (Sentry)


- **Integration:** Backend initialized with Sentry
- **Captures:** Server-side exceptions, request errors, and performance metrics

```js
// server/src/index.js
import * as Sentry from '@sentry/node';
tracesSampleRate: 1.0 });
