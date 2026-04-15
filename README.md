
# Medical Aid Membership Management System (WinDev)

##  Project Overview
This project is a Membership Management System developed using WinDev.  
It allows a Medical Aid Company to manage Principal Members and their Dependents, calculate premiums, and generate reports.

---

## ⚙️ Features

### 👤 Principal Member Management
- Auto-generated Membership Number
- Capture:
  - First Name
  - Surname
  - Date of Birth
  - Postal Address
  - Date Joined
- Benefit Date automatically calculated (+90 days)
- Default Status set to **NEW**
- Default Premium set to **0**

---

### 👨‍👩‍👧 Dependent Management
- Each Principal Member can have **0 to many dependents**
- Dependent is linked to Principal Member
- Dependent cannot exist without Principal Member
- Membership Number is automatically inherited

---

### 💰 Premium Calculation
Premium is calculated based on number of dependents:

- 0 dependents → ₹100  
- 1–2 dependents → ₹100 + ₹75 per dependent  
- 3 or more dependents → ₹100 + ₹50 per dependent  

#### Membership Status:
- Premium < ₹200 → **ACTIVE**
- Premium ≥ ₹200 → **PENDING**

---

### 📊 Report Generation
Displays:
- First Name
- Surname
- Date Joined
- Benefit Date
- Membership Status
- Premium

Additional:
- Agent Fee = 5% of Premium
- Total Premium and Total Agent Fee at bottom

---

### 💾 CSV Export (Extra Task)
- Principal member data can be exported to a comma-separated file (.csv)

---

## 🛠️ Technologies Used
- WinDev
- HFSQL Database

---

## ▶️ How to Run the Project
1. Open WinDev
2. Click on **Open Project**
3. Select the project folder
4. Run the main window using **GO (F5)**

---

## 👩‍💻 Author
Purva Pawar

---

## ✅ Conclusion
This system efficiently manages medical memberships, ensures correct premium calculation, and maintains structured data for reporting and export.
