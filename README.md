# 🏨 StayLuxe – Hotel Management System

A full-stack hotel management web application where customers can explore and book hotels, hotel owners can manage their properties, and administrators can manage the platform.

## Project Team

| Name | GitHub |
|---|---|
| Lakshya Sharma | [@lakshya6935](https://github.com/lakshya6935) |
| Miheeka | [@miheeka04](https://github.com/miheeka04) |

## Live Demo

[View StayLuxe](https://hotel-management-system-murex-six.vercel.app/customer/index.html)

## About the Project

StayLuxe is designed to make hotel booking and management easier through separate interfaces for customers, hotel owners, and administrators.

### Main Features

**Customer**
- Browse and search hotels.
- View hotel details, rooms, and prices.
- Register, log in, and book rooms.
- View and manage bookings.

**Hotel Owner**
- Register and log in to the owner portal.
- Add and manage hotels and rooms.
- View and manage customer bookings.
- Access the dashboard after admin approval.

**Admin**
- Manage users and hotel owners.
- Approve or reject hotel listings.
- Manage hotels and bookings.
- Access the admin dashboard through a separate login.

## Tech Stack

- Frontend: HTML, CSS, JavaScript
- Backend: Python, Flask
- Database: MongoDB Atlas / MongoDB
- Authentication: JWT
- Deployment: Vercel (frontend), Render (backend)

## Project Structure

```
StayLuxe/
├── backend/
│   ├── app.py
│   ├── config.py
│   ├── db.py
│   ├── seed.py
│   ├── requirements.txt
│   ├── routes/
│   └── utils/
│
├── frontend/
│   ├── assets/
│   │   ├── css/
│   │   └── js/
│   ├── customer/
│   ├── owner/
│   └── admin/
│
└── README.md
```

## Run the Project Locally

### 1. Clone the repository

```bash
git clone https://github.com/lakshya6935/StayLuxe.git
cd StayLuxe
```

### 2. Set up the backend

```bash
cd backend
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

For Windows, activate the environment using:

```bash
venv\Scripts\activate
```

Create a `.env` file using the provided `.env.example` and configure your MongoDB connection string and secret keys.

Start the backend:

```bash
python seed.py
python app.py
```

The Flask API runs on port 5000 by default.

### 3. Start the frontend

Open another terminal:

```bash
cd frontend
python3 -m http.server 5500
```

Open the customer website:

http://localhost:5500/customer/index.html

Owner portal:

http://localhost:5500/owner/login.html

Admin portal:

http://localhost:5500/admin/login.html

## Team Contributions

This project was developed collaboratively by Lakshya Sharma and Miheeka.

Both contributors can contribute to the codebase, improve features, and maintain the project through GitHub.

## License

This project was created for educational and portfolio purposes.

| Role | Email | Password |
|---|---|---|
| Admin | admin@stayluxe.com | Admin@12345 |
| Hotel Owner | owner@stayluxe.com | Owner@123 |
| Customer | *(register your own via the site)* | — |
