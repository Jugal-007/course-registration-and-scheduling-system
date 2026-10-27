# CRSS Security & Access Control Policy (FR-02)

## 1. Authentication Security Standards
In accordance with IEEE 830 functional requirements for the Course Registration and Scheduling System (CRSS), user authentication requires strict credential validation and brute-force counter-measures.

### 1.1 Account Lockout Specification (FR-02)
- **Failure Threshold**: Five (5) consecutive unsuccessful authentication attempts.
- **Lockout Duration**: Exactly fifteen (15) minutes from the fifth failed attempt.
- **Notification**: Automated institutional alert email dispatched to the student's registered address.
- **Administrative Override**: Authorized registrars may reset lockout state via the Admin Dashboard (`FR-18`).

### 1.2 Password Complexity Mandates
- Minimum length: 8 characters (Recommended 12+).
- Character sets required:
  - At least one uppercase Latin letter (`A-Z`)
  - At least one lowercase Latin letter (`a-z`)
  - At least one decimal numeral (`0-9`)
  - At least one special ASCII symbol (`!@#$%^&*()-_=+`)

### 1.3 Transport Layer Security
All credential submission must occur over TLS 1.3 encryption with HTTP Strict Transport Security (HSTS) headers enabled.
