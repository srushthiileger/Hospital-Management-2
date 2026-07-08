# 🏥 Hospital Management System

A full-stack **Hospital Management System** developed using **React.js**, **Node.js**, **Express.js**, and **MongoDB Atlas**. The application helps hospitals manage patient records efficiently by providing complete **CRUD (Create, Read, Update, Delete)** functionality with a clean and responsive user interface.

---

# 📌 Project Overview

This project allows hospital staff to:

- Admit new patients
- View all patient records
- Search patients by name or disease
- Filter patients by admission status
- Update patient information
- Discharge patients
- Delete patient records
- View paginated patient lists
- Switch between Light Mode and Dark Mode

The backend is built using **Express.js** and **MongoDB Atlas**, while the frontend is built using **React.js**.

---

# 🚀 Technologies Used

## Frontend

- React.js
- JavaScript (ES6)
- CSS3
- Fetch API

## Backend

- Node.js
- Express.js
- MongoDB Atlas
- Mongoose
- CORS

## Database

- MongoDB Atlas (Cloud Database)

---

# 📂 Project Structure

```
Hospital-Management-System
│
├── backend
│   ├── index.js
│   └── package.json
│
├── frontend
│   ├── src
│   │   ├── App.jsx
│   │   ├── App.css
│   │   └── main.jsx
│   │
│   ├── package.json
│   └── vite.config.js
│
└── README.md
```

---

# ✨ Features

## Patient Registration

- Admit new patients
- Automatically stores admission date
- Validates required fields

---

## View Patients

- Display all patient records
- Pagination support
- Latest patients displayed first

---

## Search

Search patients by:

- Patient Name
- Disease

---

## Filter

Filter patients by status:

- All Patients
- Admitted
- Discharged

---

## Edit Patient

Update patient information including:

- Name
- Age
- Gender
- Disease
- Doctor Assigned
- Room Number
- Status

---

## Discharge Patient

Clicking **Discharge**:

- Changes status to **Discharged**
- Automatically stores discharge date

---

## Delete Patient

Remove patient records permanently from the database.

---

## Dark Mode

Switch between:

- 🌞 Light Mode
- 🌙 Dark Mode

---

## Responsive Design

Works on:

- Desktop
- Laptop
- Tablet
- Mobile Devices

---

# 📋 Patient Information Stored

Each patient record contains:

| Field | Description |
|--------|-------------|
| Name | Patient Name |
| Age | Patient Age |
| Gender | Male/Female/Other |
| Disease | Patient Disease |
| Doctor Assigned | Doctor Name |
| Room Number | Hospital Room |
| Status | Admitted/Discharged |
| Admission Date | Date of Admission |
| Discharge Date | Date of Discharge |

---

# 🛠 Backend API

## 1. Create Patient

### POST

```
POST /patients
```

### Request Body

```json
{
  "name": "Ramesh Kumar",
  "age": 45,
  "gender": "Male",
  "disease": "Dengue",
  "doctorAssigned": "Dr. Iyer",
  "roomNumber": "204"
}
```

---

## 2. Get All Patients

### GET

```
GET /patients
```

Supports:

- Pagination
- Search
- Status Filter

Example:

```
GET /patients?page=1&limit=5
```

Search Example

```
GET /patients?search=fever
```

Filter Example

```
GET /patients?status=Admitted
```

---

## 3. Get Patient by ID

```
GET /patients/:id
```

---

## 4. Update Patient

```
PUT /patients/:id
```

Example

```json
{
    "doctorAssigned":"Dr. Mehta",
    "roomNumber":"302"
}
```

---

## 5. Discharge Patient

```
PUT /patients/:id
```

```json
{
   "status":"Discharged"
}
```

---

## 6. Delete Patient

```
DELETE /patients/:id
```

---

# 🔍 API Validation

The backend validates:

- Required fields
- Positive age
- Invalid requests
- Missing patient records

Returns proper HTTP status codes:

- 200 OK
- 201 Created
- 400 Bad Request
- 404 Not Found
- 500 Internal Server Error

---

# ⚙️ Installation

## Step 1

Clone the repository

```bash
git clone https://github.com/yourusername/Hospital-Management-System.git
```

---

## Step 2

Move to backend

```bash
cd backend
```

Install dependencies

```bash
npm install
```

Start backend

```bash
node index.js
```

Server runs at

```
http://localhost:5000
```

---

## Step 3

Move to frontend

```bash
cd frontend
```

Install dependencies

```bash
npm install
```

Run project

```bash
npm run dev
```

Frontend runs at

```
http://localhost:5173
```

---

# 🌐 MongoDB Atlas

The project uses **MongoDB Atlas** for cloud database storage.

Connection is established using **Mongoose** inside:

```
backend/index.js
```

---

# 🎨 Frontend Screens

The application contains:

- Patient Registration Form
- Edit Patient Form
- Search Bar
- Status Filter
- Patient List
- Pagination
- Dark Mode Toggle
- Responsive Layout

---

# 📮 Postman Testing

This project includes:

- Postman Collection
- Postman Environment

You can import both into **Postman** to test every API endpoint.

Available API operations:

- Create
- Read
- Update
- Delete
- Search
- Filter

---

# 🔒 Future Improvements

- User Authentication
- JWT Login
- Admin Dashboard
- Doctor Management
- Appointment Booking
- Billing System
- Medical Reports
- File Upload
- Email Notifications
- Dashboard Analytics
- Role-Based Access Control

---

# 📚 Learning Concepts Used

- React Hooks
- useState
- useEffect
- Fetch API
- REST API
- Express Routing
- CRUD Operations
- MongoDB Atlas
- Mongoose Models
- Pagination
- Search
- Filtering
- Form Validation
- Responsive CSS
- Dark Mode

---

# 👩‍💻 Author

**Srushthi Ileger**

Bachelor of Computer Applications (BCA)

---

# 📄 License

This project is developed for **educational and learning purposes only**.
