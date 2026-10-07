# 🦷 Krupa's Dental Hospital — Modern Care. Smarter Booking.

🚀 **Live Demo:** [https://arasadaanishkarthik.github.io/Krupa-Dental/](https://arasadaanishkarthik.github.io/Krupa-Dental/)

## 🏷️ Badges

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-F7DF1E?logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-18%2B-339933?logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-5-000000?logo=express&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-Database-003B57?logo=sqlite&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/Frontend-GitHub%20Pages-222222?logo=github&logoColor=white)
![License](https://img.shields.io/badge/License-ISC-blue)

## 🌟 About the Project

**Krupa's Dental Hospital** is a modern dental clinic website combined with a real appointment booking backend. The project allows patients to view the dental hospital website, select an available date and time, provide their details, and book an appointment through the system. A protected admin dashboard allows the clinic administrator to manage appointments, view booking statistics, filter appointments, and cancel bookings. The backend uses **Node.js, Express, and SQLite**, with application-level and database-level protection against double booking.

## ✨ Key Features

- 🦷 **Dental Hospital Website** — Modern responsive website for the clinic.
- 📅 **Online Appointment Booking** — Patients can book available appointments directly.
- ⏰ **30-Minute Time Slots** — Appointments are generated in 30-minute intervals.
- 🗓️ **Clinic Schedule** — Booking availability is handled for Monday–Saturday, 9 AM–8 PM.
- 🚫 **Double-Booking Protection** — Prevents two confirmed appointments from occupying the same date and time.
- 🗄️ **SQLite Database** — Appointment data is stored locally in `data/dental.db`.
- 🔐 **Protected Admin Dashboard** — Appointment management requires administrator authentication.
- 📊 **Admin Statistics** — View total confirmed, today's, and upcoming appointments.
- 🔎 **Appointment Filtering** — Filter bookings by date and status.
- ❌ **Appointment Cancellation** — Admins can cancel bookings and free the corresponding time slot.
- 🔄 **Automatic Dashboard Refresh** — The admin dashboard refreshes appointment information every 30 seconds.
- 👨‍⚕️ **Centralized Clinic Information** — Doctor/owner and contact information can be managed from one configuration file.
- 📱 **Responsive Frontend** — Designed for desktop and mobile browsing.
- 🎨 **Modern Glassmorphism UI** — Uses a navy/gold visual style with translucent interface elements.

## 🛠️ Tech Stack

### Frontend

- **HTML5**
- **CSS3**
- **JavaScript**
- Responsive web design
- Glassmorphism styling

### Backend

- **Node.js**
- **Express.js**
- **Express Session**
- **bcryptjs**
- **dotenv**

### Database

- **SQLite**
- **better-sqlite3**

### Deployment

- **GitHub Pages** for the provided live frontend
- Node.js-compatible hosting for the full backend

## 📁 Project Structure

```text
Krupa-Dental/
│
├── data/
│   └── dental.db                 # SQLite appointment database
│
├── public/
│   ├── admin/
│   │   ├── login.html            # Admin login page
│   │   └── dashboard.html        # Appointment management dashboard
│   │
│   ├── js/
│   │   ├── site-config.js        # Central clinic/owner/contact configuration
│   │   └── apply-site-config.js  # Applies site configuration across pages
│   │
│   ├── index.html                # Main website homepage
│   ├── appointment.html          # Patient appointment booking page
│   └── ...                       # Other website assets/pages
│
├── routes/
│   ├── appointments.js           # Appointment availability and booking APIs
│   └── admin.js                  # Admin authentication and management APIs
│
├── scripts/
│   └── hash-password.js          # Generates secure admin password hashes
│
├── .gitignore                    # Git ignored files
├── db.js                         # SQLite database initialization
├── package.json                  # Project dependencies and scripts
├── package-lock.json             # Locked dependency versions
├── server.js                     # Express server entry point
├── slots.js                      # Clinic hours and slot generation logic
└── README.md                     # Project documentation
