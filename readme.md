# 🏥 Hospital Management System

A full-stack web application designed to streamline end-to-end hospital operations, from patient registration to billing and record management.

## 📋 Overview

The Hospital Management System is a comprehensive solution that digitizes and automates various hospital operations. It provides an integrated platform for managing patient records, appointments, billing, bed availability, and staff management, ensuring efficient healthcare delivery and administrative processes.

## ✨ Features

### Patient Management
- **Patient Registration**: Complete patient registration with demographic and medical history
- **Medical Records**: Secure storage and retrieval of patient medical records
- **Inpatient Management**: Track and manage admitted patients
- **Outpatient Management**: Handle outpatient appointments and consultations

### Hospital Operations
- **Bed Management**: Real-time tracking of bed availability across different wards
- **Appointment Scheduling**: Book and manage patient appointments with doctors
- **Billing System**: Automated billing and invoice generation for treatments and services
- **Staff Management**: Manage doctors, nurses, and administrative staff information

### Administrative Features
- **Dashboard**: Overview of hospital operations and key metrics
- **Reports**: Generate various reports for administrative and analytical purposes
- **Search & Filter**: Quick search functionality for patients, staff, and records

## 🛠️ Tech Stack

### Frontend
- **React.js**: User interface development
- **JavaScript**: Client-side scripting
- **HTML/CSS**: Structure and styling

### Backend
- **Node.js**: Server-side runtime environment
- **Express.js**: Web application framework
- **RESTful APIs**: For client-server communication

### Database
- **MySQL**: Relational database for data storage
- Structured database design for patients, staff, appointments, billing, and bed management

## 📁 Project Structure
```
Hospital-Management-System/
│
├── backend/                # Backend server code
│   ├── config/            # Database and app configuration
│   ├── controllers/       # Request handlers and business logic
│   ├── middleware/        # Custom middleware functions
│   ├── models/            # Database models
│   ├── routes/            # API route definitions
│   ├── server.js          # Entry point for backend server
│   └── package.json       # Backend dependencies
│
├── client/                # Frontend React application
│   ├── public/            # Static files
│   ├── src/               # React source code
│   │   ├── components/    # Reusable React components
│   │   ├── pages/         # Page components
│   │   └── App.js         # Main React component
│   └── package.json       # Frontend dependencies
│
├── miniproject_dump.sql  # Database schema and initial data
│  
│
├── .gitignore            # Git ignore rules
└── README.md             # Project documentation
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- MySQL (v8.0 or higher)
- npm or yarn package manager

### Installation

1. **Clone the repository**
```bash
   git clone https://github.com/channabasappa164/Hospital-Management-System.git
   cd Hospital-Management-System
```

2. **Set up the database**
```bash
   # Login to MySQL
   mysql -u root -p
   
   # Create database and import schema
   CREATE DATABASE dbms_proj;
   USE dbms_proj;
   SOURCE backend/miniproject_dump.sql;
```

3. **Configure Backend**
```bash
   cd backend
   
   # Install dependencies
   npm install
   
   # Create .env file
   cp .env.example .env
   
   # Edit .env with your database credentials
   # DB_HOST=localhost
   # DB_PORT=3306
   # DB_USER=admin
   # DB_PASSWORD=your_password
   # DB_NAME=dbms_proj
```

4. **Configure Frontend**
```bash
   cd ../client
   
   # Install dependencies
   npm install
```

### Running the Application

1. **Start the Backend Server**
```bash
   cd backend
   npm start
   # Server runs on http://localhost:3306
```

2. **Start the Frontend Development Server**
```bash
   cd client
   npm start
   # Application runs on http://localhost:3000
```

3. **Access the Application**
   - Open your browser and navigate to `http://localhost:3000`

## 🎯 Key Functionalities

### For Patients
- Register and create patient profiles
- Book appointments with doctors
- View medical history and prescriptions
- Access billing and payment information

### For Hospital Staff
- Manage patient admissions and discharges
- Update medical records and prescriptions
- Track bed availability in real-time
- Generate bills and invoices
- View patient appointment schedules

### For Administrators
- Manage hospital staff (doctors, nurses, admin)
- Monitor overall hospital operations
- Generate analytical reports
- Oversee billing and financial records


## 📊 Database Schema

The system uses a relational database with the following main entities:
- **Patients**: Patient demographic and contact information
- **Doctors**: Medical staff details and specializations
- **Appointments**: Scheduling and appointment tracking
- **Beds**: Bed allocation and availability
- **Billing**: Financial transactions and invoices
- **Medical Records**: Patient treatment history and prescriptions
- **Inpatient/Outpatient**: Admission and consultation records


**Note**: This project was developed as part of the Database Management Systems coursework at PES University.