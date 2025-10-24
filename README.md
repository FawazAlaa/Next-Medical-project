🩺 MedReminder
A comprehensive healthcare management platform that bridges the gap between medical professionals and patients, providing seamless communication, appointment scheduling, and medical record management.

📋 Table of Contents
Overview
Features
Tech Stack
Getting Started
Test Accounts
Project Structure
API Documentation
Deployment
Contributing
🎯 Overview
MedReminder is a modern, full-stack healthcare application designed to streamline medical practice management and enhance patient care coordination. The platform serves as a digital bridge between healthcare providers and patients, offering role-based access, real-time scheduling, and comprehensive medical record management.

Key Benefits
For Medical Professionals: Streamlined patient management, appointment scheduling, and medical record keeping
For Patients: Easy access to medical records, appointment reminders, and treatment tracking
For Healthcare Systems: Improved efficiency, reduced administrative burden, and enhanced patient outcomes
✨ Features
👨‍⚕️ For Medical Professionals
Patient Management Dashboard: Comprehensive view of all patients with filtering and search capabilities
Appointment Scheduling: Advanced calendar system for managing patient appointments
Medical Records Management:
Patient case documentation
Diagnosis tracking and management
Treatment plan creation and monitoring
Medical report generation
Patient Communication: Direct communication channel with patients
Profile Management: Complete doctor profile with specialty and contact information
Analytics Dashboard: Overview of daily appointments, total patients, and pending reviews
🧑‍🦰 For Patients
Appointment Management: View and manage upcoming medical appointments
Medical Records Access: Secure access to personal medical history and diagnoses
Treatment Tracking: Monitor prescribed treatments and medications
Doctor Communication: Direct communication with healthcare providers
Profile Management: Personal profile with medical information
Reminder System: Automated reminders for appointments and medication schedules
🔐 Authentication & Security
Role-Based Access Control: Separate interfaces for medical professionals and patients
Secure Authentication: JWT-based authentication with role verification
Data Privacy: Secure handling of sensitive medical information
Session Management: Automatic session handling and logout functionality
🎨 User Experience
Responsive Design: Mobile-first approach with Tailwind CSS
Modern UI Components: Built with Radix UI and custom components
Interactive Elements: Smooth animations and transitions
Accessibility: WCAG compliant design patterns
Real-time Updates: Live data synchronization across the platform
🛠️ Tech Stack
Frontend
Framework: Next.js 15.4.6 with App Router
Language: TypeScript 5
Styling: Tailwind CSS 4
UI Components:
Radix UI - Accessible component primitives
Lucide React - Icon library
React Aria Components - Advanced accessibility
State Management: Redux Toolkit with React Redux
Form Handling: React Hook Form
Date Management: React Day Picker & date-fns
HTTP Client: Axios with interceptors
Notifications: React Toastify
Backend & Data
Mock API: Fast API for development
Data Format: JSON-based data structure
API Architecture: RESTful API design
Development Tools
Package Manager: npm
Linting: ESLint with Next.js configuration
Type Checking: TypeScript strict mode
Build Tool: Next.js built-in bundler with Turbopack support
Version Control: Git
Additional Libraries
PDF Generation: jsPDF for medical reports
Phone Input: React Phone Number Input
Payment Inputs: React Payment Inputs
Table Management: TanStack Table
Tree Components: Headless Tree
🚀 Getting Started
Prerequisites
Node.js 18+
npm or yarn package manager
Installation
Clone the repository

git clone <https://github.com/AbdElRahman-SaadElDin/MedReminer.git>
cd MedReminder
Install dependencies

npm install
Start the development server

npm run dev
Access the application

http://localhost:3000
Available Scripts
npm run dev - Start development server with Turbopack
npm run build - Build for production
npm run start - Start production server
npm run lint - Run ESLint
🔐 Test Accounts
For testing and demonstration purposes, the following demo accounts are available to explore the platform's functionality:

👨‍⚕️ Doctor Account
Email: abdelrahmansaad@gmail.com
Password: SaadSaadSaad@@777
Role: Medical Professional
Access Level: Full administrative access
Available Features:
Patient management dashboard
Appointment scheduling and calendar
Medical records management
Diagnosis and treatment tracking
Patient communication tools
Analytics and reporting
🧑‍🦰 Patient Account
Email: mazen@gmail.com
Password: SaadSaadSaad@@777
Role: Patient
Access Level: Patient portal access
Available Features:
View upcoming appointments
Access personal medical records
Track treatment progress
Communicate with healthcare providers
Manage personal profile
Receive appointment reminders
📁 Project Structure
medreminder/
├── src/
│   ├── app/                    # Next.js App Router
│   │   ├── (routes)/          # Route groups
│   │   │   ├── dashboard/     # Dashboard pages
│   │   │   ├── login/         # Authentication
│   │   │   ├── signup/        # User registration
│   │   │   ├── profile/       # User profiles
│   │   │   └── patients/      # Patient management
│   │   ├── components/        # Page-specific components
│   │   ├── funcs/            # Utility functions
│   │   └── globals.css       # Global styles
│   ├── components/           # Reusable components
│   │   └── ui/              # UI component library
│   ├── lib/                 # Core libraries
│   │   ├── interfaces/      # TypeScript interfaces
│   │   ├── store/          # Redux store
│   │   └── utils.ts        # Utility functions
│   └── interceptor/        # HTTP interceptors
├── public/                # Static assets
└── package.json          # Dependencies and scripts
🔌 API Documentation
The application uses a Fast API for mock API endpoints:

Fast API Repo: https://github.com/AbdElRahman-SaadElDin/FastAPI
Authentication Endpoints
POST /doctors - Register new doctor
POST /patients - Register new patient
GET /doctors?email={email} - Get doctor by email
GET /patients?phone={phone} - Get patient by phone
Patient Management
GET /doctors/{code}/patient - Get doctor's patients
POST /doctors/{code}/patient - Add new patient
PUT /doctors/{code}/patient/{id} - Update patient
DELETE /doctors/{code}/patient/{id} - Remove patient
Medical Records
POST /doctors/{code}/patient/{id}/cases - Add diagnosis
DELETE /doctors/{code}/patient/{id}/cases/{index} - Remove diagnosis
🚀 Deployment
Vercel Deployment (Recommended)
API Base URL: https://fast-api-dnk5.vercel.app/
App Demo Link: https://medreminder-bay.vercel.app/
Alternative Deployment Options
Netlify: Static site deployment
Railway: Full-stack deployment with database
Docker: Containerized deployment
🤝 Contributing
Fork the repository
Create a feature branch (git checkout -b feature/feature-one)
Commit your changes (git commit -m 'Add feature-one')
Push to the branch (git push origin feature/feature-one)
Open a Pull Request
Development Guidelines
Follow TypeScript best practices
Use conventional commit messages
Ensure responsive design
Add proper error handling
Write meaningful component documentation
📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgments
Built with modern web technologies for optimal performance
Designed with accessibility and user experience in mind
Inspired by the need for better healthcare communication tools
