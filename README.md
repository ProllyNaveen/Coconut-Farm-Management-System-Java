# 🥥 Coconut Farm Management System

A Java desktop application for managing coconut farm operations. Built with NetBeans, MySQL, and JasperReports as part of an Enterprise Application Development (EAD) coursework.

---

## 📋 About

The Coconut Farm Management System helps agriculture offices track and manage coconut farming activities across multiple farms and seasons. It connects three types of users — Admins, Farmers, and Field Officers — in one unified system.

---

## 👥 User Roles

| Role | Responsibilities |
|---|---|
| **Admin** | Manage seasons, manage users, view dashboard, generate reports |
| **Farmer** | Register plots, log farming activities, record harvests |
| **Field Officer** | Conduct farm inspections, record health status, give recommendations |

---

## ✨ Features

- Role-based login system
- Season management (Yala, Maha etc.)
- Coconut plot registration and management
- Farming activity logging (fertilizing, irrigation, pest control, pruning)
- Field inspection recording with health status tracking
- Harvest entry with quality grading
- Admin dashboard with key performance indicators
- Seasonal crop performance report using JasperReports

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Language | Java |
| IDE | NetBeans |
| Database | MySQL |
| Reporting | JasperReports / Jaspersoft Studio |
| Version Control | Git / GitHub |

---

## 🗄️ Database

Database name: `coconut_farm_db`

**Tables:**
- `user` — all system users (admin, farmer, field officer)
- `season` — growing seasons
- `plot` — farmer coconut plots
- `activity` — farming activities per plot per season
- `inspection` — field officer inspection records
- `harvest` — harvest entries per plot per season

---

## 🏗️ Project Structure

```
src/
 └── coconut/
      ├── db/          → Database connection (Singleton pattern)
      ├── model/       → Plain Java model classes
      ├── dao/         → Database operations (DAO pattern)
      └── ui/
           ├── LoginForm
           ├── admin/   → Admin screens
           ├── farmer/  → Farmer screens
           └── officer/ → Field Officer screens
```

---

## ⚙️ Setup Instructions

1. Clone the repository
```bash
git clone https://github.com/ProllyNaveen/CoconutFarmMS.git
```

2. Open the project in NetBeans

3. Import the database
   - Open MySQL Workbench
   - Run `coconut_farm_db.sql` from the `database/` folder

4. Add MySQL connector JAR to project libraries
   - Right click project → Properties → Libraries → Add JAR

5. Run the project

---

## 🔑 Default Login Credentials

| Role | Username | Password |
|---|---|---|
| Admin | admin01 | admin123 |
| Farmer | farmer01 | farmer123 |
| Field Officer | officer01 | officer123 |

---

## 📊 Reports

The system includes a **Seasonal Coconut Yield & Inspection Report** generated using JasperReports. This report joins data from farmer, plot, inspection, and harvest tables to help admins make decisions on resource allocation for the next season.

---

## 🎓 Academic Info

- **Module:** Enterprise Application Development (EAD)
- **Tool:** NetBeans, MySQL, JasperReports

---
