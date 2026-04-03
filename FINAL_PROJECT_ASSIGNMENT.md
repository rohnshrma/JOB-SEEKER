# Job Portal System using MERN Stack (MongoDB, Express, React, Node)

## Final MERN Stack Capstone Project

**Institute Name:** WebiGeeks  
**Tagline:** Build Like a Real Developer

---

## 1. Cover Page

# Job Portal System using MERN Stack (MongoDB, Express, React, Node)

## Final MERN Stack Capstone Project

**Institute Name:** WebiGeeks  
**Tagline:** Build Like a Real Developer

---

## 2. Introduction

### What is this project?
The **Job Portal System using MERN Stack** is a full-stack web application where:

- Job seekers can register, build profiles, search jobs, and apply
- Recruiters can post jobs and manage applicants
- Admins can monitor users, jobs, and platform activity

This project is designed as a **final capstone project** for MERN students who have already completed projects such as a Food Ordering App and an E-commerce App.

### Why is a Job Portal important in the real world?
A job portal is a practical and industry-relevant system because it includes:

- Authentication and authorization
- CRUD operations
- File upload handling
- Search and filtering
- Dashboard-based workflows
- Role-based access control
- API integration
- Real-world database relationships

This makes it an excellent project for becoming job-ready as a MERN developer.

---

## 3. Learning Outcomes

By completing this final capstone project, students will be able to:

- Build a complete full-stack MERN application
- Design and structure RESTful APIs
- Implement secure JWT-based authentication
- Create role-based authorization for multiple user types
- Integrate React frontend with Express and MongoDB backend
- Design scalable MongoDB schemas and relationships
- Handle resume or file uploads
- Build protected routes and dashboards
- Deploy a complete MERN application
- Create a strong portfolio project aligned with industry expectations

---

## 4. Tech Stack

The project should be built using:

- **MongoDB**
- **Express.js**
- **React.js**
- **Node.js**
- **JWT Authentication**
- **Mongoose**
- **bcryptjs**
- **React Router**
- **Axios or Fetch API**
- **Multer**
- **Cloudinary** (optional for file uploads)

---

## 5. Features Breakdown

### A. User (Job Seeker)

Students must build the following features for the Job Seeker role:

- Register
- Login
- Logout
- Create profile
- Edit profile
- Upload resume
- Search jobs
- Filter jobs by category, location, or type
- View job details
- Apply to jobs
- Track application status

### B. Recruiter

Students must build the following features for the Recruiter role:

- Register/Login as recruiter
- Create company or recruiter profile
- Post a new job
- Edit job
- Delete job
- View all posted jobs
- View applicants for each job
- Accept applicants
- Reject applicants

### C. Admin

Students must build the following features for the Admin role:

- Login as admin
- Manage all users
- Manage all jobs
- Delete inappropriate users or jobs
- View total users
- View total jobs
- View total applications
- Access dashboard statistics

---

## 6. Project Phases

## Phase 1: Project Setup

### Task List
- Create `client` and `server` folders
- Initialize React app
- Initialize Node/Express backend
- Install required packages
- Setup environment variables
- Create GitHub repository

### What Student Should Build
- Basic MERN project structure
- Running frontend and backend setup

### Expected Output
- React app starts successfully
- Express server runs successfully
- Initial folder structure is ready

---

## Phase 2: Backend Setup (Express + MongoDB)

### Task List
- Setup Express server
- Connect MongoDB using Mongoose
- Add middleware
- Configure routing
- Setup basic error handling

### What Student Should Build
- Working backend architecture connected with MongoDB

### Expected Output
- MongoDB connection is successful
- Test API route works in Postman

---

## Phase 3: Database Design

### Task List
- Design User schema
- Design Job schema
- Design Application schema
- Add timestamps
- Create model relationships

### What Student Should Build
- Well-structured Mongoose models for all entities

### Expected Output
- Models ready for authentication, job posting, and applications

---

## Phase 4: Authentication (JWT)

### Task List
- Build register API
- Build login API
- Hash passwords using bcryptjs
- Generate JWT tokens
- Protect private routes

### What Student Should Build
- Secure authentication system

### Expected Output
- Users can register and login successfully
- Protected routes work with token verification

---

## Phase 5: Role-based Access

### Task List
- Add role field in user model
- Create middleware for role checking
- Restrict routes for recruiter and admin
- Protect dashboard access by role

### What Student Should Build
- Role-based authorization system

### Expected Output
- Only authorized users can access role-specific routes

---

## Phase 6: Job APIs

### Task List
- Create job posting API
- Create get all jobs API
- Create get single job API
- Create update job API
- Create delete job API
- Add search and filter support

### What Student Should Build
- Full Job Management module

### Expected Output
- Recruiters can manage jobs
- Users can browse available jobs

---

## Phase 7: Application System

### Task List
- Create apply-to-job API
- Prevent duplicate applications
- Fetch logged-in user's applications
- Fetch applicants for recruiter jobs
- Update application status

### What Student Should Build
- Job application workflow

### Expected Output
- Job seekers can apply
- Recruiters can manage applicants and status

---

## Phase 8: File Upload

### Task List
- Implement resume upload
- Validate file format and size
- Save file using local storage or Cloudinary
- Link uploaded resume to user profile

### What Student Should Build
- Resume upload system

### Expected Output
- Users can upload and update resume successfully

---

## Phase 9: Frontend (React)

### Task List
- Setup React Router
- Build pages and reusable components
- Create forms for login/register/profile/job posting
- Connect APIs to frontend
- Show loading and error states

### What Student Should Build
- Full frontend for all roles

### Expected Output
- Frontend communicates correctly with backend APIs

---

## Phase 10: Admin Dashboard

### Task List
- Build admin dashboard UI
- Show user and job statistics
- Show all users
- Show all jobs
- Add delete/manage functionality

### What Student Should Build
- Admin control panel

### Expected Output
- Admin can manage platform data from dashboard

---

## Phase 11: Deployment

### Task List
- Deploy frontend
- Deploy backend
- Connect production MongoDB database
- Add environment variables
- Test live project

### What Student Should Build
- Production-ready deployed MERN app

### Expected Output
- Project is live and accessible through deployed link

---

## 7. Folder Structure

```text
job-portal-system/
│
├── client/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── context/
│   │   ├── services/
│   │   ├── utils/
│   │   ├── App.js
│   │   └── main.js / index.js
│
├── server/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── utils/
│   ├── uploads/
│   ├── app.js
│   └── server.js
│
├── .env
├── package.json
└── README.md
```

### Important Folders
- `/client` → React frontend
- `/server` → Node and Express backend
- `/models` → Database models
- `/routes` → API routes
- `/controllers` → Business logic
- `/components` → Reusable UI components
- `/pages` → Screen-level React pages

---

## 8. Database Schema

### A. User Schema
Suggested fields:

- `name`
- `email`
- `password`
- `role` (`jobseeker`, `recruiter`, `admin`)
- `phone`
- `skills`
- `education`
- `experience`
- `resume`
- `profileImage`
- `companyName`
- `createdAt`
- `updatedAt`

### B. Job Schema
Suggested fields:

- `title`
- `description`
- `companyName`
- `location`
- `salary`
- `jobType`
- `experienceLevel`
- `skillsRequired`
- `postedBy`
- `deadline`
- `status`
- `createdAt`
- `updatedAt`

### C. Application Schema
Suggested fields:

- `job`
- `applicant`
- `resume`
- `coverLetter`
- `status` (`pending`, `accepted`, `rejected`)
- `appliedAt`
- `updatedAt`

### Relationship Notes
- One recruiter can post many jobs
- One job can receive many applications
- One job seeker can apply to many jobs

---

## 9. API Endpoints Table

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/auth/register` | Register user |
| POST | `/api/auth/login` | Login user |
| GET | `/api/auth/profile` | Get logged-in user profile |
| PUT | `/api/auth/profile` | Update logged-in user profile |
| POST | `/api/upload/resume` | Upload resume |
| GET | `/api/jobs` | Get all jobs |
| GET | `/api/jobs/:id` | Get single job details |
| POST | `/api/jobs` | Create job |
| PUT | `/api/jobs/:id` | Update job |
| DELETE | `/api/jobs/:id` | Delete job |
| GET | `/api/jobs/recruiter/my-jobs` | Get recruiter's jobs |
| POST | `/api/applications/:jobId/apply` | Apply to a job |
| GET | `/api/applications/my-applications` | Get user's applications |
| GET | `/api/applications/job/:jobId` | Get applicants for a job |
| PUT | `/api/applications/:id/status` | Update application status |
| GET | `/api/admin/users` | Get all users |
| GET | `/api/admin/jobs` | Get all jobs |
| DELETE | `/api/admin/user/:id` | Delete user |
| DELETE | `/api/admin/job/:id` | Delete job |
| GET | `/api/admin/stats` | Get dashboard statistics |

---

## 10. UI Pages Required

Students must create the following pages:

- Home Page
- Register Page
- Login Page
- User Profile Page
- Edit Profile Page
- Job Listing Page
- Job Details Page
- Applied Jobs Page
- Recruiter Dashboard
- Post Job Page
- Edit Job Page
- Applicants Page
- Admin Panel
- Admin Dashboard
- Not Found Page

### UI Tip
Use clean layout, simple navigation, and separate dashboards based on user role.

---

## 11. Bonus Features

Students can add the following advanced features:

- Pagination
- Dark Mode
- Notifications
- Real-time updates using Socket.io
- Saved jobs
- Advanced filters
- Company logo upload
- Interview scheduling
- Search suggestions

---

## 12. Submission Requirements

Students must submit:

- GitHub repository link
- Live deployed project link
- Screenshots of all major pages
- `README.md` file
- Short project description
- API documentation or Postman collection

### README.md should include:
- Project title
- Features
- Tech stack
- Installation steps
- Environment variables
- API overview
- Deployment link
- Screenshots

---

## 13. Evaluation Rubric

| Component | Marks |
|---|---:|
| Backend Development | 20 |
| Frontend Development | 20 |
| Authentication and Authorization | 15 |
| Database Design | 15 |
| Features Completion | 20 |
| Deployment and Documentation | 10 |
| **Total** | **100** |

### Evaluation Criteria
Students will be evaluated on:

- Code quality
- Folder structure
- Working features
- API design
- UI clarity
- Authentication and security
- Deployment success
- Documentation quality

---

## 14. Timeline

## 12-Day Project Plan

| Day | Work Focus |
|---|---|
| Day 1 | Setup project, install dependencies, MongoDB connection |
| Day 2 | Models, routes, controllers structure |
| Day 3 | Registration and login APIs |
| Day 4 | JWT auth and protected routes |
| Day 5 | Job CRUD APIs |
| Day 6 | Application system APIs |
| Day 7 | React setup and routing |
| Day 8 | Login, register, home, jobs pages |
| Day 9 | Profile and recruiter dashboard integration |
| Day 10 | Admin dashboard integration |
| Day 11 | Testing, polishing, deployment preparation |
| Day 12 | Deployment, README, screenshots, final submission |

### Simplified Timeline
- **Day 1-2** → Backend
- **Day 3-4** → Auth
- **Day 5-6** → APIs
- **Day 7-8** → Frontend
- **Day 9-10** → Integration
- **Day 11-12** → Deployment

---

## 15. Instructions for Students

- Follow clean coding practices
- Use proper naming conventions
- Keep frontend and backend modular
- Test APIs before connecting frontend
- Use environment variables for secrets
- Protect role-based routes properly
- Validate inputs on frontend and backend
- Push code regularly to GitHub
- Focus on core features first
- Attempt bonus features only after completing required modules

### Small Tips for Students
- Start with backend first
- Build one feature at a time
- Test every module after completing it
- Avoid writing all code in one file
- Keep UI simple and professional
- Think about how you will explain this project in an interview

---

## Final Note

This capstone project is designed to simulate a real-world full-stack application. Students are expected to approach it professionally, write clean code, and build a project that is portfolio-ready.

This is not just an academic task. It is your opportunity to build like a real developer.

**WebiGeeks**  
**Build Like a Real Developer**

---

## Important Submission Policy

- This project must be submitted within **15 days**
- Students must **not use AI for application logic, backend logic, authentication logic, database design logic, API logic, or core project decision-making**
- AI may be used only for:
- HTML structure assistance
- CSS styling assistance
- Dummy data generation
- Students must fully understand and explain the code they submit
- Plagiarized, copied, or AI-generated logic-based submissions may be rejected
- **Course certification depends on the successful completion and submission of this final project**

### Final Instruction
Treat this project as your practical exam, portfolio piece, and industry preparation assignment. Your certification will be based on your ability to build, explain, and submit this project properly within the given timeline.
