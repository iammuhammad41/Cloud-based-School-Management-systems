```markdown
# Cloud‑Based School Management System  
**Oracle 10g/11g Forms & Reports**

A scalable, cloud‑hosted application to manage all aspects of K‑12 and higher‑education operations—student admissions, staff records, attendance, grading, billing, library, transport, and reporting—built with Oracle Forms & Reports on a 10g/11g database backend.

---

## ⚠️ Confidentiality Notice  
Most form modules and library files are **not** included here due to client‑side copyright and confidentiality constraints.  
If you require the complete source under NDA, please contact the project owner.

---

## 📂 Repository Structure  
```

/
├── README.md                ← this file
├── login\_test.fmb           ← login form source
├── login\_test.fmx           ← login form executable
└── sql/                     ← (schema & seed scripts; public versions)

````

> **Note:** All other `.fmb/.fmx` modules (student, teacher, attendance, etc.) have been omitted.

---

## 🏗️ Main Modules & Forms  

| Module                        | Source Form       | Executable Form    | Description                                           |
|:------------------------------|:------------------|:-------------------|:------------------------------------------------------|
| **1. Login & Security**       | `login_test.fmb`  | `login_test.fmx`   | User authentication, single‑sign‑on, role‑based access |
| **2. Student Management**     | _confidential_    | _confidential_     | Admission, profile, guardians, transfers              |
| **3. Teacher & Staff Mgmt.**  | _confidential_    | _confidential_     | HR records, assignments, leave tracking               |
| **4. Class Scheduling**       | _confidential_    | _confidential_     | Timetable creation, room allocation                   |
| **5. Attendance Tracking**    | _confidential_    | _confidential_     | Daily attendance, late marks, SMS notifications       |
| **6. Grading & Report Cards** | _confidential_    | _confidential_     | Exam entry, grade calculation, transcript generation  |
| **7. Fee & Billing**          | _confidential_    | _confidential_     | Fee structures, invoicing, payment tracking           |
| **8. Library Management**     | _confidential_    | _confidential_     | Catalog, check‑in/out, fines                          |
| **9. Transport & Routing**    | _confidential_    | _confidential_     | Bus routing, stops, driver assignment                 |
| **10. User & Role Admin.**    | _confidential_    | _confidential_     | Manage user accounts, roles, privileges               |

---

## 🚀 Quick Start  

1. **Database Setup**  
   - Run `sql/schema.sql` to create tables, indexes, sequences.  
   - Run `sql/seed_data.sql` for lookup values (roles, classes, fee types).

2. **Compile & Deploy Forms**  
   - Open `login_test.fmb` in Oracle Forms Developer → **Compile** → generate `login_test.fmx`.  
   - Place all `.fmx` files on your Forms Server (e.g. `$ORACLE_HOME/forms/java`).

3. **Configure Web Listener**  
   - In `formsweb.cfg`, add a section for each form.  
   - Ensure `FORMS_PATH` points to your deployment folder.

4. **Run the Application**  
   - Access via browser:
     ```
     http://<forms-server>:<port>/forms/frmservlet?
       config=schoolConfig
       &form=login_test.fmx
     ```

---

## 📞 Support  
For access to the full suite of modules or custom integrations, please reach out under your existing support agreement.  
````
