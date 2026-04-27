# JeevRakshak

JeevRakshak (Life Saver) is a full-stack web application designed to bridge the gap between patients and emergency care through seamless technology. It features portals for patients and hospitals, allowing for quick response to emergencies, SOS alerts, health tracking, and digital prescriptions.

## Features

### Patient Portal
- **Dashboard & Health Tracker**: Track daily goals like steps, water intake, and sleep.
- **Emergency SOS**: Single-click SOS button that instantly alerts the nearest operational hospital with the patient's current location.
- **Doctor on Call**: Request consultations based on symptom urgency (Low, Medium, High).
- **Prescriptions View**: Access digital prescriptions issued by hospitals.
- **BMI Calculator**: Calculate and track Body Mass Index.
- **Nearby Services**: Locate nearby clinics and pharmacies.

### Hospital Portal
- **Dashboard & Patient Management**: View admitted patients and their details.
- **Emergency Response Queue**: View and resolve incoming SOS and doctor consultation requests from nearby patients.
- **Digital Prescriptions**: Prescribe medications directly to patients via the portal.
- **Staff Management**: Add and remove hospital staff members.

### Admin Controls
- **Hospital Verification**: Admins can review and approve hospital registrations before they become operational, ensuring trust and validity. Approval sends an automated email with login credentials.

## Technology Stack
- **Frontend**: HTML5, CSS3, Vanilla JavaScript.
- **Backend**: Node.js, Express.js.
- **Database**: MongoDB (Native Node Driver).
- **Authentication**: JSON Web Tokens (JWT), Bcrypt.
- **Other Tools**: Nodemailer (for approval emails).

## Project Structure
```text
JeevRakshak/
├── Jeevrakshak/               # Frontend Code (HTML, CSS, JS)
│   ├── login.html             # Common Login / Registration
│   ├── patient.html           # Patient Dashboard
│   ├── hospital.html          # Hospital Dashboard
│   └── ...                    # Associated CSS/JS assets
├── jeevrakshak-backend/       # Backend Node.js Server
│   ├── server.js              # Main Express Application & API Routes
│   ├── package.json           # Backend Dependencies
│   └── .env                   # Environment Variables
```

## Setup & Installation

### 1. Prerequisites
- [Node.js](https://nodejs.org/) installed on your machine.
- A MongoDB cluster or local MongoDB server.
- An email account for Nodemailer (e.g., Gmail with App Passwords enabled).

### 2. Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd jeevrakshak-backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Ensure you have a `.env` file in the `jeevrakshak-backend` directory and configure the following variables:
   ```env
   PORT=3000
   MONGO_URI="your_mongodb_connection_string"
   JWT_SECRET="your_secure_jwt_secret"
   EMAIL_USER="your_email@gmail.com"
   EMAIL_PASS="your_email_app_password"
   ```
4. Start the server:
   ```bash
   npm start
   ```

### 3. Frontend Setup
1. You can simply open the `Jeevrakshak/login.html` file in your preferred web browser, or use a local development server (like Live Server in VS Code) to serve the frontend files.
2. Ensure the frontend JS files are configured to point to the correct backend API URL (default is usually `http://localhost:3000`).

## Contributors
- Ayush Tripathi
- Ashish Ashok Gunapache
- Dhruv G Nayak
- Dhyan Sirigeri
