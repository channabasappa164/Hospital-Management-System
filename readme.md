# 🏥 Hospital Management System

A full-stack web application designed to streamline end-to-end hospital operations, from patient registration to billing and record management across multiple hospitals.

## 📋 Overview

The Hospital Management System is a comprehensive solution that digitizes and automates various hospital operations across three major hospitals: City General Hospital, Downtown Medical Center, and Green Valley Hospital. It provides an integrated platform for managing patient records, appointments, billing, bed availability, staff management, and medical services, ensuring efficient healthcare delivery and administrative processes.

## ✨ Features

### Patient Management
- **Patient Registration**: Complete patient registration with demographic details, blood type, and medical history
- **Patient Portal**: Secure login system for patients to access their records
- **Medical Records Management**: Secure storage and retrieval of patient medical records and reports
- **Inpatient Management**: Track and manage admitted patients with room assignments
- **Outpatient Management**: Handle outpatient consultations and appointments
- **Patient Classification**: Automatic categorization as In-Patient or Out-Patient

### Hospital Operations
- **Multi-Hospital Support**: Manage operations across 3 hospitals with different specializations
- **Bed Management**: Real-time tracking of bed availability across 12 different room types
  - Single, Double, Suite, and ICU rooms
  - Automated availability updates via database triggers
  - Capacity tracking for each room
- **Room Assignment System**: Automated room allocation based on availability
- **50+ Medical Services**: Comprehensive service catalog including:
  - Surgical procedures (Cardiac, Orthopedic, Pediatric, Emergency)
  - Diagnostic services (Radiology, Pathology, Endoscopy)
  - Specialized care (Oncology, Neurology, Cardiology)
  - Emergency services (Trauma, Stroke, Burn treatment)
- **Department Management**: 6 specialized departments across hospitals
  - Cardiology, Orthopedics, Pediatrics, Surgery, Emergency, Neurology

### Staff Management
- **Doctor Management**: Track doctors with specializations and department assignments
- **Nurse Management**: Manage nursing staff across different wards and hospitals
- **Employee Records**: Comprehensive employee database with contact information
- **Staff-Patient Assignment**: Link medical staff to patient care

### Billing & Financial
- **Automated Billing System**: Generate bills for room assignments and services
- **Multiple Payment Methods**: Support for Cash, Credit Card, Debit Card, and EMI
- **Service-based Pricing**: Individual pricing for each medical service
- **Room-based Charges**: Pricing based on room type (₹100 - ₹600 per day)
- **Billing History**: Complete transaction history with timestamps

### Administrative Features
- **Dashboard**: Overview of hospital operations and key metrics
- **Real-time Updates**: Automatic room availability updates using database triggers
- **Visitor Management**: Track and manage patient visitors
- **Insurance Integration**: Store patient insurance provider information
- **Emergency Contacts**: Quick access to patient emergency contact information

## 🛠️ Tech Stack

### Frontend
- **React.js**: User interface development
- **JavaScript**: Client-side scripting
- **HTML/CSS**: Structure and styling
- **Responsive Design**: Mobile and desktop compatibility

### Backend
- **Node.js**: Server-side runtime environment
- **Express.js**: Web application framework
- **RESTful APIs**: For client-server communication
- **Middleware**: Custom authentication and validation

### Database
- **MySQL 9.0.1**: Relational database management system
- **Database Triggers**: Automated room availability management
- **Foreign Keys**: Ensuring referential integrity
- **Complex Relationships**: Multiple interconnected tables

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

# 🏥 Hospital Management System

A full-stack web application designed to streamline end-to-end hospital operations, from patient registration to billing and record management across multiple hospitals.

## 📋 Overview

The Hospital Management System is a comprehensive solution that digitizes and automates various hospital operations across three major hospitals: City General Hospital, Downtown Medical Center, and Green Valley Hospital. It provides an integrated platform for managing patient records, appointments, billing, bed availability, staff management, and medical services, ensuring efficient healthcare delivery and administrative processes.

## ✨ Features

### Patient Management
- **Patient Registration**: Complete patient registration with demographic details, blood type, and medical history
- **Patient Portal**: Secure login system for patients to access their records
- **Medical Records Management**: Secure storage and retrieval of patient medical records and reports
- **Inpatient Management**: Track and manage admitted patients with room assignments
- **Outpatient Management**: Handle outpatient consultations and appointments
- **Patient Classification**: Automatic categorization as In-Patient or Out-Patient

### Hospital Operations
- **Multi-Hospital Support**: Manage operations across 3 hospitals with different specializations
- **Bed Management**: Real-time tracking of bed availability across 12 different room types
  - Single, Double, Suite, and ICU rooms
  - Automated availability updates via database triggers
  - Capacity tracking for each room
- **Room Assignment System**: Automated room allocation based on availability
- **50+ Medical Services**: Comprehensive service catalog including:
  - Surgical procedures (Cardiac, Orthopedic, Pediatric, Emergency)
  - Diagnostic services (Radiology, Pathology, Endoscopy)
  - Specialized care (Oncology, Neurology, Cardiology)
  - Emergency services (Trauma, Stroke, Burn treatment)
- **Department Management**: 6 specialized departments across hospitals
  - Cardiology, Orthopedics, Pediatrics, Surgery, Emergency, Neurology

### Staff Management
- **Doctor Management**: Track doctors with specializations and department assignments
- **Nurse Management**: Manage nursing staff across different wards and hospitals
- **Employee Records**: Comprehensive employee database with contact information
- **Staff-Patient Assignment**: Link medical staff to patient care

### Billing & Financial
- **Automated Billing System**: Generate bills for room assignments and services
- **Multiple Payment Methods**: Support for Cash, Credit Card, Debit Card, and EMI
- **Service-based Pricing**: Individual pricing for each medical service
- **Room-based Charges**: Pricing based on room type (₹100 - ₹600 per day)
- **Billing History**: Complete transaction history with timestamps

### Administrative Features
- **Dashboard**: Overview of hospital operations and key metrics
- **Real-time Updates**: Automatic room availability updates using database triggers
- **Visitor Management**: Track and manage patient visitors
- **Insurance Integration**: Store patient insurance provider information
- **Emergency Contacts**: Quick access to patient emergency contact information

## 🛠️ Tech Stack

### Frontend
- **React.js**: User interface development
- **JavaScript**: Client-side scripting
- **HTML/CSS**: Structure and styling
- **Responsive Design**: Mobile and desktop compatibility

### Backend
- **Node.js**: Server-side runtime environment
- **Express.js**: Web application framework
- **RESTful APIs**: For client-server communication
- **Middleware**: Custom authentication and validation

### Database
- **MySQL 9.0.1**: Relational database management system
- **Database Triggers**: Automated room availability management
- **Foreign Keys**: Ensuring referential integrity
- **Complex Relationships**: Multiple interconnected tables

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
│   ├── miniproject_dump.sql  # Database schema and initial data
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
   CREATE DATABASE miniproject;
   USE miniproject;
   SOURCE backend/miniproject_dump.sql;
```

3. **Configure Backend**
```bash
   cd backend
   
   # Install dependencies
   npm install
   
   # Create .env file
   touch .env
   
   # Add the following to .env file:
   DB_HOST=localhost
   DB_PORT=3306
   DB_USER=admin
   DB_PASSWORD=your_password
   DB_NAME=miniproject
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
- Register with complete demographic and medical information
- Secure login to access personal medical records
- View medical history, test reports, and prescriptions
- Access billing information and payment history
- Update emergency contact and insurance details

### For Medical Staff (Doctors & Nurses)
- Access patient medical records
- Update patient reports and prescriptions
- Manage patient assignments
- Track inpatient admissions and room assignments
- View department-specific patient lists

### For Hospital Administrators
- Manage multiple hospitals (3 hospitals in system)
- Monitor bed availability across 12 room types in real-time
- Oversee 50+ medical services
- Manage 17+ employees including doctors and nurses
- Generate bills for room assignments and services
- Track patient admissions and discharges
- View comprehensive billing and financial records
- Manage visitor access to patients

## 📊 Database Schema

The system uses a relational MySQL database with the following structure:

### Main Tables

**Patients** (Primary entity)
- Patient ID (Primary Key)
- Personal Information: Name, DOB, Sex, Blood Type
- Contact: Phone, Email, Address, Emergency Contact
- Insurance Provider
- Patient Type: In-Patient / Out-Patient
- Secure Password for login
- Auto-generated timestamp

**Hospitals** (3 hospitals)
- Hospital ID, Name, Location
- Specializations
- Contact Information

**Departments** (6 departments)
- Department ID, Name, Description
- Location within hospital
- Linked to specific hospitals

**Doctors** (5 doctors)
- Doctor ID, Name, DOB, Sex
- Specialization
- One-to-one relationship with Department

**Nurses** (12 nurses)
- Nurse ID, Name, DOB, Sex
- Ward/Location assignment
- Linked to Employee and Hospital

**Employees** (17 employees)
- Employee ID, Name, Address
- Phone Number, Sex
- Base table for all staff

**Rooms** (12 rooms across hospitals)
- Room ID, Type (Single/Double/Suite/ICU)
- Location, Capacity
- Real-time Availability status
- Pricing (₹100 - ₹600)
- Hospital association

**Services** (50 services)
- Service ID, Name, Description
- Location, Hospital
- Pricing (₹100 - ₹7,500)
- Categories: Surgery, Diagnostics, Consultations, Emergency Care

**Inpatient** (Admission records)
- Inpatient ID, Patient ID
- Hospital Name, Room ID
- Employee (Nurse) assignment
- Admission Date
- **Automated Triggers for room availability**

**Medical_Records**
- Record Number, Patient ID
- Employee ID (Doctor/Nurse)
- Medical Report details
- Test results and prescriptions

**Bills** (112+ transactions)
- Bill ID, Patient ID
- Amount, Payment Method
- Auto-generated Timestamp
- Linked to services and room assignments

**Visitors**
- Visitor ID, Name, Sex
- Phone Number
- Patient association

### Database Features

- **Foreign Key Constraints**: Maintains referential integrity across all tables
- **Automated Triggers**: 
```sql
  -- Trigger 1: Update room availability after patient admission
  update_room_availability_after_assignment
  
  -- Trigger 2: Update room availability after patient discharge
  update_room_availability_after_discharge
```
- **Cascade Operations**: Proper handling of related data
- **Multi-Hospital Architecture**: Support for multiple hospitals with shared services
- **Real-time Bed Tracking**: Automatic availability updates based on capacity



## 🔄 Automated Systems

### Room Availability Management
The system uses MySQL triggers to automatically manage room availability:

1. **After Patient Admission**:
   - Counts occupied beds in the assigned room
   - If room reaches capacity, sets availability to 0 (unavailable)

2. **After Patient Discharge**:
   - Counts remaining patients in the room
   - If room has available capacity, sets availability to 1 (available)

### Billing Automation
- Automatic bill generation for room assignments
- Service-based billing with predefined prices
- Support for multiple payment methods

## 📈 System Capabilities

- **Multi-Hospital Management**: 3 hospitals with different specializations
- **Comprehensive Service Catalog**: 50+ medical services
- **Staff Management**: 17 employees (5 doctors, 12 nurses)
- **Room Management**: 12 rooms with automatic availability tracking
- **Patient Records**: Complete medical history and reports
- **Financial Tracking**: 112+ billing transactions recorded
- **Department Organization**: 6 specialized departments




**Note**: This project was developed as part of the Database Management Systems coursework at PES University.