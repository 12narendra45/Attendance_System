# Attendance System

A modern attendance management system built for employee check-in/check-out using React, Express, and Supabase. The application supports employee attendance marking with location tracking, admin authentication, employee registration, report generation, and LOP management.

## Overview

This project helps organizations track employee attendance efficiently with:
- Employee attendance marking through a web interface
- GPS-based location validation
- PIN verification for secure attendance actions
- Admin login and secure operations
- Employee management
- Monthly and daily attendance report exports
- Leave Without Pay (LOP) marking

---

## Table of Contents

| Section | Description |
|---|---|
| Features | Core application capabilities |
| Tech Stack | Technologies used in the project |
| Screenshots | UI previews of the application |
| Installation | Setup instructions |
| Environment Variables | Required configuration |
| Usage | How to use the application |
| Project Structure | Main folders and responsibilities |
| API Modules | Backend functionality |
| Contributing | How to contribute |
| License | Project license |

---

## Features

| Feature | Description |
|---|---|
| Employee Attendance | Employees can mark attendance with department and status selection |
| Location Tracking | Uses browser geolocation to capture employee location during attendance |
| PIN Verification | Adds a second layer of verification before marking attendance |
| Admin Login | Secure admin authentication using employee ID and password |
| Add Employee | Admin can add new employees with ID, name, department, and PIN |
| Attendance Reports | Download monthly Excel reports |
| Daily Sheets | Download daily attendance reports in Excel format |
| LOP Management | Admin can mark loss of pay entries for employees |
| Employee List | View and manage employee details from the admin panel |

---

## Tech Stack

| Category | Technology |
|---|---|
| Frontend | React + Vite |
| Backend | Node.js + Express |
| Database | Supabase |
| Styling | Tailwind CSS |
| Excel Export | xlsx |
| Authentication | JWT + bcryptjs |
| Routing | React Router DOM |

---

## Screenshots



| Home / Attendance Screen | Admin Dashboard |
|---|---|
| <img src="./images/attendance-home.png" alt="Attendance Home Screen" width="420" /> | <img src="./images/admin-dashboard.png" alt="Admin Dashboard" width="420" /> |

| Add Employee Form | Attendance Report Export |
|---|---|
| <img src="./images/add-employee.png" alt="Add Employee Form" width="420" /> | <img src="./images/report-export.png" alt="Attendance Report Export" width="420" /> |

| Daily Attendance Sheet |  |
|---|---|
| <img src="./images/daily-sheet.png" alt="Daily Attendance Sheet" width="420" /> |  |



## Installation

### Prerequisites
- Node.js 18+
- npm
- Supabase account
- Git

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/attendance-system.git
cd attendance-system
```

### 2. Install Backend Dependencies
```bash
cd backend
npm install
```

### 3. Install Frontend Dependencies
```bash
cd ../frontend/attandance-marker
npm install
```

### 4. Configure Environment Variables
Create a `.env` file inside the backend folder:

```env
PORT=5000
FRONTEND_URL=http://localhost:5173
SUPABASE_URL=your_supabase_url
SUPABASE_ANON_KEY=your_supabase_anon_key
SUPABASE_SERVICE_ROLE_KEY=your_service_role_key
JWT_SECRET=your_jwt_secret
```

### 5. Start the Backend
```bash
cd backend
npm start
```

### 6. Start the Frontend
```bash
cd frontend/attandance-marker
npm run dev
```

The application should now run locally.

---

## Environment Variables

| Variable | Required | Description |
|---|---|---|
| PORT | Yes | Backend server port |
| FRONTEND_URL | Yes | Frontend base URL for CORS |
| SUPABASE_URL | Yes | Supabase project URL |
| SUPABASE_ANON_KEY | Yes | Supabase anonymous key |
| SUPABASE_SERVICE_ROLE_KEY | Yes | Supabase service role key |
| JWT_SECRET | Yes | Secret key for JWT token signing |

---

## Usage

### Employee Flow
1. Open the application home page
2. Select department
3. Select employee ID
4. Choose attendance status
5. Allow location access
6. Enter PIN when prompted
7. Submit attendance

### Admin Flow
1. Open the admin login modal
2. Enter employee ID and password
3. Access admin dashboard
4. Add new employee records
5. Download monthly or daily reports
6. Mark LOP entries for employees

---

## Project Structure

```text
attendance-system/
├── backend/
│   ├── config/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── .env
│   ├── package.json
│   └── server.js
│
├── frontend/
│   └── attandance-marker/
│       ├── public/
│       ├── src/
│       ├── package.json
│       ├── vite.config.js
│       └── index.html
│
├── netlify.toml
├── README.md
└── package.json
```

---

## API Modules

| Module | Purpose |
|---|---|
| Admin Routes | Admin login and protected access |
| Employee Routes | Employee registration and management |
| Attendance Routes | Marking attendance and PIN verification |
| Report Routes | Monthly and daily attendance data export |
| LOP Routes | Leave without pay tracking |

---

## Features Summary

| Module | Description |
|---|---|
| Attendance | Track employee working status |
| Admin Panel | Manage employee records and reports |
| Reports | Generate Excel exports |
| Security | JWT and PIN verification |
| Data Storage | Supabase cloud database |

---

## Contributing

Contributions are welcome. To contribute:

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to your branch
5. Open a pull request

---

## License

This project is licensed under the MIT License.

---



## Contact

For support or questions, please contact the project maintainer or open an issue in the repository.
