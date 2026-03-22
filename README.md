# NMC Virtual Pharmacy

A virtual pharmacy management system designed specifically for NUST hostelites. This application provides a convenient alternative to the NUST Medical Center (NMC), allowing students to access medicines and emergency services directly from their rooms.

---

### 📦 Stack

- **C++** (Core logic and source code)
- **Qt Framework** (Cross-platform GUI design)
- **MySQL** (Database for user and inventory management)
- **SQL Queries** (Data retrieval and manipulation)

---

### ✨ Quick start

```bash
# Clone the repository
git clone https://github.com/ZainAbid-1/NMC-pharm.git

# Build the project using make
make

# Run the application
./NMC-pharm
```

*Note: Ensure you have the Qt development environment and MySQL server configured on your local machine.*

---

### 🚀 System Features

- **Account-Based System** — Secure sign-in and sign-up functionality for different user roles.
- **Admin Portal** — Specialized dashboard for pharmacy staff to manage inventory and logistics.
- **User-Side Interface** — Intuitive shopping experience for hostelites to browse and buy medicines.
- **Quick Ambulance Service** — Emergency request system that forwards location data to the admin portal.
- **Location Integration** — Direct links to Google Maps for pharmacy and hostel navigation.

---

### 🎹 Portals & Controls

- **Admin Menu** — View incoming orders, update stock levels, adjust medicine prices, and manage active ambulance calls.
- **Client Menu** — Search the medicine store, request an ambulance, view "About Us" information, and submit feedback.
- **Persistence** — All transactions and stock updates are reflected in real-time across both portals via the central database.

---

### 🤖 How it works

The system architecture follows a classic Client-Server-Database model:

1.  **Authentication** — Users enter credentials on the Login Page, which are validated against the MySQL database.
2.  **Order Flow** — When a user selects medicine, the data is stored in a database table. The Admin Portal polls this table to "View Orders" and process them.
3.  **Emergency Logic** — An ambulance call prompts the user for a location (hostel by default), which is immediately forwarded as a high-priority alert to the Admin Portal.
4.  **Inventory Management** — Admins update stock/prices via GUI forms that execute `UPDATE` SQL queries, instantly refreshing the "Store" view for all users.

---
