# Course Registration and Scheduling System (CRSS)

A modern, responsive web-based platform for academic course registration, schedule planning, prerequisite verification, and conflict detection developed in accordance with IEEE 830 Software Requirements Specifications.

---

## 📌 Project Overview
The **Course Registration and Scheduling System (CRSS)** provides a centralized digital environment for higher education institutions. It streamlines the student enrollment workflow, assists faculty in managing section capacities and course rosters, and gives academic administrators fine-grained control over catalog definitions and timetable clash detection.

### Key Stakeholders & Personas
- **Students**: Browse course offerings, inspect prerequisites, construct weekly schedules, add/drop/swap sections, and view enrollment status.
- **Faculty**: Monitor real-time section enrollments, inspect class rosters, and submit midterm/final grades.
- **Academic Administration**: Define course catalogs, manage credit-hour policies, configure enrollment windows, and resolve venue/instructor scheduling collisions.

---

## 🎯 Functional Requirements Breakdown (IEEE 830)

| Requirement ID | Module | Description |
| :--- | :--- | :--- |
| **FR-01** | Authentication | Secure student and faculty authentication using institutional credentials. |
| **FR-02** | Security & Lockout | Multi-tier brute-force prevention: 15-minute account lockout after 5 consecutive failed login attempts. |
| **FR-03** | Course Catalog | Searchable and filterable academic course catalog with syllabus metadata. |
| **FR-04** | Prerequisite Engine | Automated validation preventing enrollment without completing prerequisite coursework. |
| **FR-05** | Conflict Detection | Real-time matrix checking to eliminate schedule and exam timetable overlaps. |
| **FR-06** | Credit Enforcement | Automated limits ensuring minimum (12) and maximum (21) credit-hour thresholds per term. |
| **FR-07** | Waitlist Engine | First-come, first-served automated queue allocation upon seat vacancies. |
| **FR-08** | Timetable Matrix | Interactive visual weekly calendar view with color-coded course blocks. |
| **FR-09** | Add / Drop / Swap | Self-service registration adjustments within university add/drop periods. |
| **FR-10** | Audit Logging | Immutable timestamped audit trails of all registration and override transactions. |

---

## 📂 Repository Structure
```text
course-registration-and-scheduling-system/
├── README.md               # Core system architecture & specification
├── SECURITY.md             # Security policies, password rules, and lockout specifications
├── login.html              # Student and faculty portal login interface
├── styles/
│   └── main.css            # Responsive layout & academic portal styling
└── scripts/
    └── auth.js             # Client-side input validation and authentication handlers
```

---

## 🛠️ Technology Stack
- **Frontend**: HTML5, Semantic CSS3, Vanilla JavaScript (ES2022)
- **Design System**: Responsive CSS Grid / Flexbox with WCAG 2.1 AA Accessibility
- **Version Control**: Git & GitHub with feature-branch workflow and Pull Request peer reviews

---

## 👨‍💻 Author & Institutional Attribution
- **Developer**: Jugal Panchal
- **Email**: jugalpanchal1125@gmail.com
- **Institution**: ITM SLS Baroda University
- **Department**: Computer Science & Engineering
- **Course**: Software Engineering & Agile Methodology Lab (Practical 6)


## ?? Authentication Module (FR-01)
The student login portal (login.html) provides role-based credential entry for students and instructors.
