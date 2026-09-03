# HR Leave Account Management System (IRCTC)

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)

An enterprise-grade, secure full-stack web application developed for **IRCTC (Indian Railway Catering and Tourism Corporation)** to digitize and automate the lifecycle of employee leave management.

## 🏢 Business Context & Problem Statement
Prior to this system, IRCTC managed employee leave accounts via manual paper registers and fragmented spreadsheets. This approach was highly prone to human error, making it difficult to accurately track cumulative carry-forwards, enforce strict ledger rules (like preventing negative balances for LAP and LHAP), and maintain a secure audit trail of changes. There was a critical need for a centralized platform to automate complex leave calculations securely.

## 🚀 Key Features & Architecture
*   **Automated Strict Ledger**: Designed an automated database ledger that dynamically calculates LAP (Leave on Average Pay) and LHAP balances. The backend strictly prevents negative balances at the PostgreSQL transaction level.
*   **Cumulative Tracking**: Built chronological carry-forward calculations. If historical entries are modified, the system recalculates subsequent balances to maintain absolute ledger integrity.
*   **Secure Role-Based Access Control (RBAC)**: Implemented JWT authentication and bcrypt password hashing, ensuring only authorized HR administrators can modify sensitive records.
*   **Immutable Audit Trail**: An `AuditLog` table immutably tracks all `ADD`, `EDIT`, and `DELETE` actions, ensuring complete accountability for every ledger modification.

## 🛠️ Tech Stack
*   **Frontend:** React.js (Vite), Tailwind CSS, Lucide Icons
*   **Backend:** Python (FastAPI)
*   **Database:** PostgreSQL (SQLAlchemy ORM)
# 🖼 Screenshots

<img src="images/1.png" width="100%"/>
<img src="images/2.png" width="100%"/>
<img src="images/3.png" width="100%"/>
<img src="images/4.png" width="100%"/>
<img src="images/5.png" width="100%"/>
<img src="images/6.png" width="100%"/>
<img src="images/7.png" width="100%"/>
<img src="images/8.png" width="100%"/>
<img src="images/9.png" width="100%"/>
<img src="images/10.png" width="100%"/>
<img src="images/11.png" width="100%"/>
<img src="images/12.png" width="100%"/>
<img src="images/13.png" width="100%"/>




---

# 🤝 Contributing

1. Fork the project
2. Create a feature branch
3. Commit your changes
4. Push branch
5. Open a Pull Request

---

# 📄 License

Distributed under the MIT License.
