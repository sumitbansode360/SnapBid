# 🔥 SnapBid – Real-Time Live Auction Platform

## 🔑 Demo Login Credentials

To make evaluation easier, test credentials are provided below.

### 👤 User Account
- **Username:** testuser1
- **Password:** test@123

- **Username:** testuser2
- **Password:** test@123

- **Username:** testuser3
- **Password:** test@123

SnapBid is a real-time live auction web application built using Django and WebSockets. The platform enables users to participate in seamless live bidding with instant updates, auction timers, and real-time notifications, ensuring a smooth and engaging auction experience.

This project focuses on **real-time systems**, **event-driven architecture**, and **accurate bidding logic**, demonstrating practical backend and WebSocket implementation.

---

## 🚀 Features

### 🔐 User Authentication
- Secure user registration and login
- Authenticated access to auctions and bidding

### 🔨 Live Auction System
- Real-time bidding using WebSockets
- Instant bid updates across all connected users
- Accurate auction flow with live synchronization

### ⏱ Auction Timer & Bidding Logic
- Time-bound auctions with countdown timers
- Auto-updates for auction status changes
- Prevents invalid or late bids

### 🔔 Live Notifications
- Real-time notifications for:
  - New bids
  - Auction start and end events
  - Status changes
- Improves user engagement and transparency

### 🎨 Responsive User Interface
- Clean and user-friendly frontend
- Built with Bootstrap
- Optimized for desktop and mobile devices

---

## 🛠 Tech Stack

### Backend
- Django
- Django Channels
- WebSockets

### Frontend
- HTML
- CSS
- Bootstrap
- JavaScript

### Database
- SQLite (development)
- Can be upgraded to PostgreSQL for production

---

## 🧠 Architecture Overview

- **HTTP** → Used for authentication, auction creation, and data fetching  
- **WebSockets** → Enables real-time bidding and live updates  
- **Django Channels** → Manages WebSocket connections and event broadcasting  
- **Consumers** → Handle bid events, timers, and notifications  

---

## ⚙️ Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/snapbid.git
cd snapbid

2. Create Virtual Environment
python -m venv venv
source venv/bin/activate   # Linux / Mac
venv\Scripts\activate      # Windows

3. Install Dependencies
pip install -r requirements.txt

4. Run Migrations
python manage.py makemigrations
python manage.py migrate

5. Create Superuser
python manage.py createsuperuser

6. Start the Server
python manage.py runserver
