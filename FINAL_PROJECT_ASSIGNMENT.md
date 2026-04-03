# Job Portal System using MERN Stack (MongoDB, Express, React, Node)

## Final MERN Stack Capstone Project

**Institute Name:** WebiGeeks  
**Tagline:** Build Like a Real Developer

---

## 1. Introduction

### What Is This Project?
The **Job Portal System using MERN Stack** is a complete full-stack web application where different users interact with the platform based on their role.

- **Job Seekers** can register, build profiles, upload resumes, search jobs, and apply for openings
- **Recruiters** can post jobs, manage listings, and review applicants
- **Admins** can monitor the platform, manage users, manage jobs, and view platform-level statistics

This project is designed as the **final capstone assignment** for MERN students who have already built projects such as a Food Ordering App and an E-commerce App. It is intended to bring together everything learned in the course into one strong, portfolio-ready system.

### Why Is a Job Portal Important in the Real World?
A job portal is one of the most practical and professional full-stack projects because it naturally includes many real software engineering concepts:

- Authentication and authorization
- CRUD operations
- Role-based dashboards
- Real database relationships
- Search and filtering
- File upload management
- API design and integration
- Protected routes and secure access

This makes it an excellent final project for students who want to become job-ready as MERN developers.

---

## 2. Learning Outcomes

By completing this capstone project, students will be able to:

- Build a complete full-stack MERN application using a structured project architecture
- Design RESTful APIs for real-world business requirements
- Implement secure JWT-based authentication and authorization
- Create role-based access control for Job Seekers, Recruiters, and Admins
- Connect a React frontend with an Express and MongoDB backend
- Design scalable MongoDB schemas and model relationships
- Handle file uploads such as resumes and profile documents
- Build responsive dashboards and protected pages
- Deploy a full-stack MERN application to a live environment
- Create a portfolio project aligned with industry expectations

---

## 3. Tech Stack

The project must be built using the following technologies:

- **MongoDB**
- **Express.js**
- **React.js**
- **Node.js**
- **JWT Authentication**
- **Mongoose**
- **bcryptjs**
- **React Router**
- **Axios** or **Fetch API**
- **Multer**
- **Cloudinary** (optional, but recommended for file upload storage)

---

## 4. Features Breakdown

### A. User Role: Job Seeker
Students must build the following features for Job Seekers:

- Register
- Login
- Logout
- Create profile
- Edit profile
- Upload resume
- Search jobs
- Filter jobs by category, location, type, or keyword
- View job details
- Apply to jobs
- Track application status

### B. User Role: Recruiter
Students must build the following features for Recruiters:

- Register and login as recruiter
- Create company or recruiter profile
- Post a new job
- Edit posted job
- Delete posted job
- View all jobs created by the recruiter
- View applicants for each job
- Accept applicants
- Reject applicants

### C. User Role: Admin
Students must build the following features for Admin:

- Login as admin
- Manage all users
- Manage all jobs
- Delete inappropriate users or job posts
- View total users
- View total jobs
- View total applications
- Access dashboard statistics

---

## 5. Project Phases

### Phase 1: Project Setup

**Task List**

- Create `client` and `server` folders
- Initialize React application
- Initialize Node and Express backend
- Install all required dependencies
- Configure environment variables
- Create GitHub repository

**What Student Should Build**

- A properly structured MERN project foundation
- Running frontend and backend setup

**Expected Output**

- React app starts successfully
- Express server runs successfully
- Initial project structure is ready

### Phase 2: Backend Setup (Express + MongoDB)

**Task List**

- Setup Express server
- Connect MongoDB using Mongoose
- Add middleware
- Configure route structure
- Setup basic error handling

**What Student Should Build**

- A working backend architecture connected to MongoDB

**Expected Output**

- MongoDB connection is successful
- Test route works in Postman

### Phase 3: Database Design

**Task List**

- Design User schema
- Design Job schema
- Design Application schema
- Add timestamps
- Define collection relationships

**What Student Should Build**

- Well-structured Mongoose models for all major entities

**Expected Output**

- Models are ready for authentication, job posting, and application flow

### Phase 4: Authentication (JWT)

**Task List**

- Build register API
- Build login API
- Hash passwords using `bcryptjs`
- Generate JWT tokens
- Protect private routes

**What Student Should Build**

- Secure authentication system

**Expected Output**

- Users can register and login successfully
- Private routes work using token verification

### Phase 5: Role-Based Access

**Task List**

- Add `role` field in User model
- Create middleware for role checking
- Restrict recruiter and admin routes
- Protect dashboard access by role

**What Student Should Build**

- Role-based authorization system

**Expected Output**

- Only authorized users can access role-specific routes

### Phase 6: Job APIs

**Task List**

- Create job posting API
- Create get all jobs API
- Create get single job API
- Create update job API
- Create delete job API
- Add search and filter support

**What Student Should Build**

- Complete job management module

**Expected Output**

- Recruiters can manage jobs
- Users can browse available jobs

### Phase 7: Application System

**Task List**

- Create apply-to-job API
- Prevent duplicate applications
- Fetch logged-in user's applications
- Fetch applicants for recruiter jobs
- Update application status

**What Student Should Build**

- Complete job application workflow

**Expected Output**

- Job seekers can apply to jobs
- Recruiters can manage applicants and update status

### Phase 8: File Upload

**Task List**

- Implement resume upload
- Validate file size and format
- Save file using local upload or Cloudinary
- Link uploaded file with user profile

**What Student Should Build**

- Resume upload system

**Expected Output**

- Users can upload and update resumes successfully

### Phase 9: Frontend (React)

**Task List**

- Setup React Router
- Build pages and reusable components
- Create forms for login, register, profile, and job posting
- Connect frontend with backend APIs
- Show loading and error states

**What Student Should Build**

- Complete frontend interface for all roles

**Expected Output**

- Frontend works correctly with backend APIs

### Phase 10: Admin Dashboard

**Task List**

- Build admin dashboard UI
- Show user and job statistics
- Show all users
- Show all jobs
- Add delete and manage functionality

**What Student Should Build**

- Admin control panel

**Expected Output**

- Admin can manage platform data from the dashboard

### Phase 11: Deployment

**Task List**

- Deploy frontend
- Deploy backend
- Connect production MongoDB database
- Configure environment variables
- Test the live application

**What Student Should Build**

- Production-ready deployed MERN application

**Expected Output**

- Fully live project with working frontend and backend

---

## 6. Recommended Folder Structure

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

### Important Core Folders

- `/client` for React frontend
- `/server` for Node and Express backend
- `/models` for database schemas
- `/routes` for API route definitions
- `/controllers` for business logic
- `/components` for reusable UI components
- `/pages` for screen-level React pages

---

## 7. Database Schema

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

## 8. API Endpoints Table

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

## 9. UI Pages Required

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
Keep the interface clean, responsive, and role-based. Navigation should clearly change depending on whether the user is a Job Seeker, Recruiter, or Admin.

---

## 10. Bonus Features

Students may add the following advanced features after completing all core requirements:

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

## 11. Submission Requirements

Students must submit the following:

- GitHub repository link
- Live deployed project link
- Screenshots of major pages
- `README.md`
- Short project description
- API documentation or Postman collection

### README Must Include

- Project title
- Features list
- Tech stack
- Installation steps
- Environment variables used
- API overview
- Deployment link
- Screenshots

---

## 12. Evaluation Rubric

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
- Feature completion
- API design
- UI clarity and usability
- Authentication and security basics
- Deployment success
- Documentation quality

---

## 13. Timeline

### 12-Day Working Plan

| Day | Work Focus |
|---|---|
| Day 1 | Project setup, dependencies, MongoDB connection |
| Day 2 | Models, controllers, route structure |
| Day 3 | Registration and login APIs |
| Day 4 | JWT authentication and protected routes |
| Day 5 | Job CRUD APIs |
| Day 6 | Application system APIs |
| Day 7 | React setup and routing |
| Day 8 | Login, register, home, and jobs pages |
| Day 9 | Profile and recruiter dashboard integration |
| Day 10 | Admin dashboard integration |
| Day 11 | Testing, bug fixing, and deployment preparation |
| Day 12 | Deployment, README, screenshots, and final polish |

### Simplified Milestone View

- **Day 1-2**: Backend
- **Day 3-4**: Authentication
- **Day 5-6**: APIs
- **Day 7-8**: Frontend
- **Day 9-10**: Integration
- **Day 11-12**: Deployment

### Final Submission Deadline

- The complete project must be submitted within **15 days**

---

## 14. Instructions for Students

- Follow clean coding practices from the beginning
- Use proper naming conventions
- Keep frontend and backend modular
- Test APIs before connecting them to the frontend
- Use environment variables for secret keys and configuration
- Protect role-based routes correctly
- Validate user input on both frontend and backend
- Push code regularly to GitHub
- Complete core features before attempting bonus features

### Small Tips for Students

- Start with backend logic first
- Build one module at a time
- Test each feature after completing it
- Avoid writing all code in one file
- Keep the UI simple, responsive, and professional
- Be prepared to explain your project in an interview

---

## 15. Important Policy and Certification Rules

### AI Usage Policy

Students must follow the following academic honesty rules strictly:

- AI must **not** be used for backend logic
- AI must **not** be used for authentication logic
- AI must **not** be used for database design logic
- AI must **not** be used for API logic
- AI must **not** be used for business logic or core project decision-making
- AI may be used only for **HTML structure assistance**
- AI may be used only for **CSS styling assistance**
- AI may be used only for **dummy data generation**

Every student must fully understand, write, and explain the project logic independently.

### Submission Rule

- This capstone project must be completed and submitted within **15 days**
- Late submissions may affect evaluation and certification status

### Certification Rule

- **Course certification depends on the successful completion and submission of this final capstone project**
- Students may be asked to explain their code, logic, architecture, and implementation decisions during review
- If a student cannot explain the submitted logic, the submission may be rejected for certification purposes

---

## Final Note

This capstone project is designed to simulate a real-world full-stack application. Students are expected to approach it professionally, write clean code, and produce a portfolio-ready result.

This is not just an assignment. It is your practical exam, your strongest classroom project, and a major step toward becoming job-ready.

**WebiGeeks**  
**Build Like a Real Developer**
