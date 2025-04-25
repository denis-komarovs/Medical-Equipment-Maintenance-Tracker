# Medical Equipment Maintenance Tracker

## Overview
**Medical Equipment Maintenance Tracker (MEMT)** is a web-based system for hospitals and clinics to manage:
- Medical equipment inventory
- Scheduled maintenance
- Fault reporting and resolution
- Vendor contact management
- Compliance-ready reporting

## Skills Learnt and/or Used
- **Laravel & PHP Development**: Built a full backend system using Laravel's MVC structure.
- **Database Management**: Designed and managed a relational MySQL database.
- **Frontend Development (Vue.js)**: Built dynamic, responsive front-end components using Vue.js.
- **API Creation**: Developed RESTful APIs to enable external systems and mobile apps to interact with the data.
- **UI/UX Design Principles**: Created a clean UI & UX experience.
- **Testing & Debugging**: Wrote automated PHPUnit tests and performed manual testing. Due to time constraints this hasnt been done properly
- **Version Control (Git)**: Used Git for version control with feature branches, clear commit messages, and organized project management.
- **Kanban/Agile Workflows**: Planned and managed project tasks using a Kanban board to simulate an Agile workflow.
- **Best Practice Coding Standards**: Followed PSR-12 coding standards and wrote clean, maintainable code.
- **Problem-Solving & Critical Thinking**: Analyzed project requirements and solved technical challenges like overdue maintenance tracking and role-based permissions.
- **Collaboration & Communication**: although I worked solo for this project I simulated teamwork qualities by writing clear documentation, reviewing code & having good project organisation

---

## Features
- **Equipment Management**: Track critical medical devices and their maintenance schedules.
- **Maintenance Scheduler**: Auto-generate and assign maintenance tasks.
- **Fault Reporting**: Staff can easily report equipment issues.
- **Vendor CRM**: Manage external service providers and their contacts.
- **Audit Reports**: Exportable maintenance logs for compliance.
- **RESTful API**: Expose equipment and maintenance data for external apps.
- **Notifications**: Email alerts for overdue maintenance.

---

## Tech Stack
- **Backend**: Laravel 10 (PHP 8.x)
- **Database**: MySQL 8.x
- **Frontend**: Vue.js components combined with Blade templates, styled using Bootstrap and TailwindCSS.
- **API**: REST (Laravel Resources & API Controllers)
- **Version Control**: Git + GitHub

---

## Project Structure
```
/app
  /Http
    /Controllers
      - DeviceController.php
      - MaintenanceController.php
      - VendorController.php
    /Requests
      - DeviceRequest.php
      - MaintenanceRequest.php
/resources
  /views
    /devices
    /maintenance
    /vendors
/routes
  - web.php
  - api.php
/database
  /migrations
  /seeders
/tests
  /Feature
  /Unit
```

---

## Installation

1. **Clone the repo**
   ```bash
   git clone https://github.com/yourusername/MEMT.git
   cd MEMT
   ```

2. **Install dependencies**
   ```bash
   composer install
   npm install && npm run dev
   ```

3. **Setup environment**
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

4. **Configure database**  
   Update your `.env` with your local DB settings:
   ```
   DB_DATABASE=memt
   DB_USERNAME=root
   DB_PASSWORD=yourpassword
   ```

5. **Run migrations**
   ```bash
   php artisan migrate --seed
   ```

6. **Serve the app**
   ```bash
   php artisan serve
   ```

---

## API Endpoints

| Method | Endpoint | Description |
| `GET` | `/api/devices` | List all equipment |
| `POST` | `/api/maintenance-logs` | Create a maintenance log |
| `GET` | `/api/vendors` | List vendors |
| `POST` | `/api/faults` | Report a new fault |

Full API documentation available at `/api/documentation` (or a Postman collection in future).

---

## Testing

Run the test suite with:
```bash
php artisan test
```

**Includes tests for:**
- Device creation
- Maintenance scheduling logic
- Fault reporting flow

---

## Agile Workflow

- Managed with **GitHub Projects** (Kanban board)
- Branch naming conventions:  
  - `feature/device-crud`
  - `feature/maintenance-api`
  - `bugfix/overdue-calculation`

- PRs created for every major feature and self-reviewed.

---

## Contribution

This project is done solo but is developed as part of a simulated real-world workflow.  
Pull Requests (PRs), detailed commit messages, and agile-style task management have been used.

---

## License

Open-source for learning purposes.

---

# Final Notes

> This project simulates the type of CRM, ERP, and database-driven solutions used by healthcare organizations and industry sectors.  

---

# Screenshots

| Main Dashboard | Equipment List | Fault Reporting |
|:---|:---|:---|
| ![](path/to/screenshot1.png) | ![](path/to/screenshot2.png) | ![](path/to/screenshot3.png) |

---

# 📍 Quick Links
- [Laravel Documentation](https://laravel.com/docs)
- [MySQL Documentation](https://dev.mysql.com/doc/)
- [Bootstrap](https://getbootstrap.com/) / [TailwindCSS](https://tailwindcss.com/)
