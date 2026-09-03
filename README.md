<h1>
  <img src="HR_Leave_Account_Management_System/frontend/public/Irctc_tourism_light.png" alt="IRCTC Logo" width="60">
   IRCTC Enterprise Web Solutions
</h1>



![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![NodeJS](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)

Welcome to the central repository for the custom enterprise solutions developed for the **Indian Railway Catering and Tourism Corporation (IRCTC)**. 

This repository operates as a monorepo containing four distinct, production-ready full-stack web applications engineered to digitize manual processes, enhance operational efficiency, and provide real-time data analytics.

---

## 📂 Repository Structure & Projects

### 1. [HR Leave Account Management System](./HR_Leave_Account_Management_System)
A secure platform to digitize the lifecycle of employee leave management.
*   **Problem Solved:** Replaced error-prone manual paper registers.
*   **Key Features:** Automated strictly-validated ledger (prevents negative balances), chronological carry-forward tracking, and immutable audit logs.
*   **Tech Stack:** React.js, Python (FastAPI), PostgreSQL, JWT Auth.

### 2. [Bharat Gaurav Train - Seat Allocation System](./BGT_Seat_Allocation_System)
A real-time charting and seat allocation engine engineered for IRCTC's custom tourist trains.
*   **Problem Solved:** Eliminated conflicts and bottlenecks when allocating seats with complex constraints (group bookings, lower berth requests).
*   **Key Features:** `Socket.IO` WebSockets for live charting updates, complex automatic seat mapping algorithms, and manual override capabilities.
*   **Tech Stack:** React.js, Python (FastAPI, Socket.IO), PostgreSQL.

### 3. [Staff Sales Tracking & Analytics Dashboard](./Staff_Sales_Tracking)
A robust data-entry dashboard to aggregate fragmented daily sales data across multiple tourism verticals.
*   **Problem Solved:** Centralized daily sales tracking and eliminated the nightmare of validating duplicate transaction IDs across disjointed Excel reports.
*   **Key Features:** Complex ACID PostgreSQL transactions, strict duplicate Transaction ID prevention, and monthly target tracking.
*   **Tech Stack:** React.js, Node.js (Express), PostgreSQL, Python Pandas.

### 4. [RAILSIGHTS - Passenger Analytics Management](./RAILSIGHTS_Passenger_Analytics_Management)
A data-intensive analytics platform providing high-speed querying and visualization of historical passenger metrics.
*   **Problem Solved:** Resolved the inability to quickly query and analyze massive legacy CSV datasets while enforcing strict data security.
*   **Key Features:** Distributed search architecture syncing PostgreSQL data to Elasticsearch via Redis, alongside granular module-level Role-Based Access Control (RBAC).
*   **Tech Stack:** React.js, Python (Flask), PostgreSQL, Elasticsearch (v8), Redis, Docker.

---

## 🛠️ Global Tech Stack

While each project is architected independently, they share a modern, scalable core stack:
*   **Frontend:** React.js (Vite / CRA), Tailwind CSS, Lucide Icons, Recharts
*   **Backend:** Python (FastAPI / Flask), Node.js (Express)
*   **Databases:** PostgreSQL (SQLAlchemy / pg)
*   **Real-time & Search:** Elasticsearch, Redis, Socket.IO
*   **Security:** JWT, bcrypt password hashing, Role-Based Access Control (RBAC)

## 🚀 Getting Started

Each project is fully containerized or includes its own localized setup instructions. Please navigate to the specific project folder and refer to its individual `README.md` to run the servers locally.
