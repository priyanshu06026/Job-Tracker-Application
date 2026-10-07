# 💼 Job Status Tracker

A modern full-stack application that helps job seekers efficiently manage and track their job applications throughout the recruitment process. Instead of maintaining spreadsheets, users can monitor application statuses, interview progress, offers, and rejections from a centralized dashboard.

---

## 🚀 Overview

Applying to multiple companies can quickly become overwhelming. Important details such as application dates, interview schedules, recruiter communications, and offer statuses often get scattered across emails, notes, and spreadsheets.

Job Status Tracker streamlines the entire process by providing a single platform to organize and visualize the job search journey.

---

## ✨ Features

### 📋 Application Management
- Add and manage job applications
- Track company and role details
- Store application dates and notes
- Update application progress

### 🔄 Status Tracking
Track applications through multiple stages:

- Applied
- Online Assessment
- Interview Scheduled
- Technical Round
- HR Round
- Offer Received
- Rejected

### 🔍 Search & Filtering
- Search by company name
- Filter by application status
- Sort applications by date
- Quick access to important records

### 📊 Dashboard Analytics
- Total applications submitted
- Interviews scheduled
- Offers received
- Rejection statistics
- Application conversion rates

### 👤 User Authentication
- Secure signup and login
- Personalized dashboard
- Protected routes

---

## 🔄 Workflow

The Job Status Tracker follows a structured recruitment pipeline that helps users manage every stage of their job search.

### Step 1: User Authentication

- User signs up or logs into the platform.
- A personalized dashboard is created for tracking applications.
- All application data is securely associated with the user's account.

### Step 2: Add a Job Application

Users can create a new application by providing:

- Company Name
- Job Role
- Application Date
- Job Link
- Notes (optional)

The application is initially assigned the status:

```text
Applied
```

---

### Step 3: Track Recruitment Progress

As the recruitment process advances, users can update application statuses.

Typical workflow:

```text
Applied
   ↓
Online Assessment
   ↓
Shortlisted
   ↓
Technical Interview
   ↓
Managerial / HR Round
   ↓
Offer Received
```

Alternative outcomes:

```text
Applied
   ↓
Rejected
```

or

```text
Applied
   ↓
Online Assessment
   ↓
Technical Interview
   ↓
Rejected
```

---

### Step 4: Manage Interviews

For each application, users can:

- Schedule interview dates
- Record interview rounds
- Store feedback and notes
- Track upcoming interviews

This helps maintain a complete history of the recruitment process.

---

### Step 5: Monitor Applications

The dashboard provides real-time insights including:

- Total Applications
- Active Applications
- Interviews Scheduled
- Offers Received
- Rejections

Users can easily identify which opportunities require follow-up.

---

### Step 6: Search and Filter

Applications can be filtered by:

- Company
- Role
- Current Status
- Application Date

This enables quick access to specific records even when managing many applications.

---

### Step 7: Analyze Progress

The analytics module helps users evaluate their job search performance by displaying:

- Interview Conversion Rate
- Offer Conversion Rate
- Applications by Status
- Monthly Application Trends

These insights help users improve their application strategy.

---

## 🏛️ System Workflow Diagram

```text
User Login
     │
     ▼
Add Application
     │
     ▼
Store in Database
     │
     ▼
Update Status
     │
     ▼
Track Interviews
     │
     ▼
Generate Dashboard Analytics
     │
     ▼
Monitor Progress & Outcomes
```

---

## 🔍 Example User Journey

```text
1. Apply to Google for SWE Intern
2. Add application to Job Status Tracker
3. Status → Applied
4. Receive OA invitation
5. Status → Online Assessment
6. Clear OA
7. Status → Technical Interview
8. Attend interviews
9. Status → Offer Received
10. Dashboard statistics update automatically
```

---

## 🛠️ Tech Stack

### Frontend
- React.js
- TypeScript
- Tailwind CSS

### Backend
- Node.js
- Express.js

### Database
- PostgreSQL

### Authentication
- JWT Authentication

### Deployment
- Vercel / Render

---

## 🏗️ System Architecture

```text
Frontend (React)
       │
       ▼
 REST API Layer
       │
       ▼
Backend (Node.js)
       │
       ▼
 PostgreSQL Database
```

---

## 📂 Project Structure

```bash
Job-Status-Tracker/
│
├── frontend/
│   ├── components/
│   ├── pages/
│   ├── hooks/
│   └── services/
│
├── backend/
│   ├── routes/
│   ├── controllers/
│   ├── middleware/
│   └── models/
│
├── database/
├── public/
└── README.md
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/aashishky2/Job-Status-Tracker.git
cd Job-Status-Tracker
```

### Install Dependencies

```bash
npm install
```

### Setup Environment Variables

Create a `.env` file:

```env
DATABASE_URL=
JWT_SECRET=
PORT=5000
```

### Run Development Server

```bash
npm run dev
```

Application will be available at:

```bash
http://localhost:3000
```

---

## 🗄️ Database Design

### Users

```sql
id
name
email
password
created_at
```

### Applications

```sql
id
user_id
company
role
status
applied_date
notes
created_at
```

### Interviews

```sql
id
application_id
round
interview_date
feedback
```

---

## 🎯 Use Cases

- College students applying for internships
- Fresh graduates seeking full-time roles
- Professionals managing multiple opportunities
- Placement season application tracking
- Personal recruitment pipeline management

---

## 📈 Key Benefits

- Eliminates manual spreadsheet tracking
- Improves organization during job search
- Provides visibility into recruitment progress
- Helps users identify application trends
- Simplifies interview management

---

## 🔮 Future Enhancements

- Email reminders for interviews
- Calendar integration
- Resume version tracking
- Recruiter contact management
- AI-powered job application insights
- Application success prediction
- Export reports to PDF/Excel

---

## 🤝 Contributing

Contributions are welcome.

1. Fork the repository

```bash
git fork
```

2. Create a new branch

```bash
git checkout -b feature/new-feature
```

3. Commit your changes

```bash
git commit -m "Add new feature"
```

4. Push to GitHub

```bash
git push origin feature/new-feature
```

5. Open a Pull Request

---

## 👨‍💻 Author

**Aashish Sharma**

GitHub: https://github.com/aashishky2

---


## 🌟 Motivation

This project was built to solve a common problem faced by students and job seekers: efficiently tracking multiple job applications and recruitment processes without relying on scattered spreadsheets or notes. The goal is to provide a structured, user-friendly platform that makes job hunting more organized and productive.
