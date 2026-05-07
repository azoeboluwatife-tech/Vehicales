# Vehicales
# Nigeria National Transport Registry (NNTR)

A prototype digital transport platform for vehicle registration, GPS-enabled fleet monitoring, and cargo tracking in Nigeria.

---

## 📌 Project Overview

The **Nigeria National Transport Registry (NNTR)** is a web-based platform designed to modernize vehicle and logistics management through:

* Vehicle registration
* Fleet management
* Cargo monitoring
* GPS-enabled tracking
* Compliance verification

This project was developed as a:

* 🎓 School project
* 🚀 Startup prototype
* 🏛️ Government proposal demo

---

## ⚠️ Important Disclaimer

This platform **does not track arbitrary vehicles using only plate numbers**.

Tracking functionality works **only for registered vehicles with authorized GPS devices or driver mobile applications installed**.

The system does **not access restricted government databases** such as:

* FRSC internal systems
* NPF databases
* National identity systems

All tracking is:

* Owner-authorized
* GPS-based
* Demonstration-only

---

# ✨ Features

## 🚗 Vehicle Registration

* Register private or commercial vehicles
* Generate vehicle records
* Assign unique tracking IDs

## 📍 GPS Vehicle Tracking

* Search vehicles using:

  * Plate number
  * VIN
  * Tracking ID
* Display vehicle location on map

## 🔐 Security & Compliance

* Authentication system
* Fleet management dashboard
* Compliance verification support

## 🗺️ Map Integration

* Google Maps integration
* Real-time location rendering

---

# 🛠️ Technologies Used

## Frontend

* HTML5
* CSS3
* Bootstrap 5
* JavaScript
* Boxicons

## Backend

* Python (Flask)

## Database

* SQLite / MySQL

## APIs & Services

* Google Maps Embed API

---

# 🧱 System Architecture

```text
GPS Device / Driver App
        ↓
 Backend API Server
        ↓
 Vehicle Database
        ↓
NNTR Web Dashboard
```

---

# 📂 Project Structure

```bash
NNTR/
│
├── index.html
├── style.css
├── login.html
├── register-form.html
├── app.py
├── database.db
├── README.md
│
├── assets/
│   ├── images/
│   └── icons/
│
└── templates/
```

---

# ⚙️ Installation

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/nntr.git
cd nntr
```

---

## 2️⃣ Install Dependencies

```bash
pip install flask
```

---

## 3️⃣ Run the Server

```bash
python app.py
```

---

## 4️⃣ Open in Browser

```text
http://127.0.0.1:5000
```

---

# 🔌 Sample API Endpoint

## Track Vehicle

```http
GET /api/track/<plate_number>
```

### Example Response

```json
{
  "plate_number": "NNTR-001",
  "latitude": 6.5244,
  "longitude": 3.3792,
  "status": "Active"
}
```

---

# 🗄️ Database Design

## Vehicles Table

| Field        | Type    |
| ------------ | ------- |
| id           | Integer |
| plate_number | String  |
| owner_name   | String  |
| vehicle_type | String  |

---

## Locations Table

| Field      | Type     |
| ---------- | -------- |
| id         | Integer  |
| vehicle_id | Integer  |
| latitude   | Float    |
| longitude  | Float    |
| timestamp  | DateTime |

---

# 🔒 Legal & Ethical Considerations

This project was developed with consideration for:

* User privacy
* Vehicle owner consent
* GPS authorization
* Ethical data handling

The system does not:

* Access confidential government databases
* Track vehicles without permission
* Provide surveillance functionality

---

# 🚀 Future Enhancements

* Mobile application
* AI route optimization
* Driver analytics
* Stolen vehicle alerts
* Logistics dashboard
* Integration with government agencies (subject to authorization)

---

# 👨‍💻 Author

Developed by Zoe Technology

---

# 📄 License

This project is for educational and demonstration purposes only.
