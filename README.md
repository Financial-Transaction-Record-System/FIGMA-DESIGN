📊 LedgerLink – Financial Transaction Record System

LedgerLink is a full-stack financial bookkeeping application designed for individuals and small businesses to manage daily income, expenses, budgets, and financial insights. It provides secure role-based access, detailed analytics, and exportable financial reports through an intuitive dashboard.


🎨 Figma UI/UX Design:
🔗 https://www.figma.com/make/aZOYvcK5BQA1bo8nmad96L/Finance-Tracking-App--Community-?t=RLvXa2Z2XHbrmnSd-1

Use this link to explore the complete UI design and layout of LedgerLink before development.


🚀 Features Overview
🔐 Authentication & Authorization

JWT-based stateless authentication

Role-Based Access Control (RBAC)

User / Accountant – Record transactions, manage budgets, view reports

Viewer / Auditor – Read-only access for verification

Admin – Manage categories, currencies, and system settings

Secure API endpoint protection

🖥️ Frontend Modules (React)
1️⃣ Transaction Entry Ledger

Add Income / Expense / Transfer

Fields: Amount, Date, Category, Payee, Notes

Recurring transactions (Rent, Subscriptions)

Receipt image upload support

2️⃣ Dashboard & Visualizations

Net Worth / Cash Flow summary cards

Expense distribution pie charts

Monthly income vs expense bar charts

3️⃣ Budgeting Tool

Category-wise monthly budget limits

Visual progress indicators

Alerts for budget threshold breaches

4️⃣ Account & Category Management

Multiple accounts (Cash, Bank, Credit Card)

Custom category hierarchy

Account balance reconciliation

5️⃣ Reports & Export

Profit & Loss statements

Filter transactions by date or category

Export data as CSV / PDF

⚙️ Backend Modules (Spring Boot)
1️⃣ User Authentication Service (SQL)

Login, Logout, Registration APIs

JWT token management

Role-based endpoint security

2️⃣ Transaction Service (MongoDB)

CRUD operations for transactions

Optimized queries by date & category

Optional multi-currency support

3️⃣ Budgeting Service (MongoDB)

Store budget limits and thresholds

Real-time remaining budget calculation

Overspending notifications

4️⃣ Account Management Service (MongoDB)

Maintain real-time account balances

Atomic transfers (Debit/Credit handling)

5️⃣ Analytics Service (MongoDB)

Aggregated data for dashboards

Financial statement generation

Receipt image storage & retrieval

🛠️ Tech Stack
Frontend

React.js

Chart.js / Recharts

Axios

JWT-based route protection

Backend

Spring Boot

Spring Security

JWT Authentication

Swagger / OpenAPI Documentation

Databases

SQL – User authentication & credentials

MongoDB – Transactions, budgets, analytics

Deployment

Frontend – Vercel

Backend – Render (Dockerized)

SQL DB – Aiven / AWS RDS / Azure SQL

NoSQL DB – MongoDB Atlas

📦 Deployment Guide
1️⃣ Frontend Deployment (Vercel)
REACT_APP_API_URL=<Backend_API_URL>


Build Command: npm run build

Output Directory: build or dist

2️⃣ Backend Deployment (Render – Docker)

Environment Variables:

SPRING_DATASOURCE_URL=<SQL_DB_URL>
MONGO_URI=<MongoDB_Atlas_URI>
JWT_SECRET=<Your_Secret_Key>

3️⃣ SQL Database Setup

Used for authentication & user data

Providers: Aiven / AWS RDS / Azure SQL

Configure tables and credentials

4️⃣ MongoDB Atlas Setup

Used for transactions, budgets, analytics

Enable network access

Create database user

Add SRV URI to backend environment

5️⃣ Final Integration

Update frontend API URL

Redeploy frontend

Verify authentication, data flow, exports

Configure custom domains (optional)

🧪 Testing & Documentation

Backend unit testing

Secure API validation

Swagger UI for API documentation

📁 Project Structure
LedgerLink/
├── frontend/        # React Application
├── backend/         # Spring Boot Application
├── docker/          # Docker configuration
├── docs/            # API documentation
└── README.md

📌 Deliverables Checklist

✅ JWT Authentication & RBAC
✅ Transaction Management with Receipts
✅ Budget Tracking with Alerts
✅ Interactive Financial Dashboard
✅ Multi-Account Support
✅ CSV / PDF Export
✅ Secure REST APIs
✅ Swagger Documentation
✅ Cloud Deployment
✅ GitHub Repository

👨‍💻 Author

Moulish Waran
Pre-final Year Engineering Student
Artificial Intelligence & Full Stack Development

📜 License

This project is licensed under the MIT License.
