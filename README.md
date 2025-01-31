# Expense-Tracker-App
The Expense Management System is a web-based application designed to assist users in tracking and managing their daily expenses. This system is built using the MERN stack (MongoDB, Express.js, React.js, and Node.js) to create a scalable, responsive, and user-friendly application.
Mini Expense Tracker with Intelligent Insights
This is a full-stack Mini Expense Tracker application that allows users to securely authenticate, manage their expenses, and receive intelligent insights about their spending patterns. It is built using ReactJS for the frontend, NodeJS for the backend, MongoDB for the database, and integrates JWT-based authentication.

 Objectives
Secure Authentication: Implement JWT-based authentication with HTTP-only cookies for secure login/logout functionality.
Expense Management: Allow users to manage their expenses (Add, Edit, Delete, View) with filtering and pagination.
Spending Insights: Provide insightful analytics about the user's spending with a chart visualization.
Light & Dark Theme Support: Implement light and dark themes for improved user experience.
Technologies Used
Frontend: ReactJS, MUI, MUI X Charts/Recharts
Backend: NodeJS, JWT-based Authentication, ExpressJS
Database: MongoDB (with Mongoose ORM)
Deployment: Vercel (Frontend), Heroku (Backend)
Methods & Approach
1. Authentication
JWT-based Authentication:
User registration with basic information (first name, last name, email, password).
Login to receive a secure JWT token stored in HTTP-only cookies.
Token expiry is handled with refresh tokens.
2. Expense Management
Expense CRUD Operations:
Users can add, update, delete, and view expenses.
Each expense has properties such as amount, category, date, and description.
Paginated expense listing with filterable options by category and date range.
3. Spending Insights
Insights Calculation:
Backend endpoint calculates total spending per category.
Generates percentage distribution of expenses across categories.
Frontend Visualization:
Pie chart or bar chart to display spending distribution across categories using MUI X Charts/Recharts.
4. Frontend (ReactJS)
Pages:
Login/Registration: Secure JWT management via HTTP-only cookies.
Dashboard: Display list of expenses with pagination, filters, and a spending insights chart.
Add/Edit Expense: Simple form for creating or editing expenses.
Delete Expense: Option to delete unwanted or duplicate expenses.
       5. Deployment
Frontend: Deployed on Vercel
Backend: Deployed on Heroku
Database: MongoDB (Hosted on MongoDB Atlas)
         API Endpoints
POST /auth/register: Register a new user.
POST /auth/login: Login a user and return a JWT token.
POST /auth/logout: Logout a user and invalidate the JWT token.
GET /expenses: Fetch paginated list of expenses with filters.
POST /expenses: Add a new expense.
PUT /expenses/:id: Edit an existing expense.
DELETE /expenses/:id: Delete an expense.
GET /insights: Fetch spending insights and analytics.
JWT Implementation
JWT tokens are used for user authentication.
The token is stored securely in HTTP-only cookies to avoid client-side access.
Tokens expire after a set time, and refresh tokens are used to handle token renewal seamlessly.
Expense Management
Expenses are stored in MongoDB with fields such as amount, category, date, and description.
API endpoints for adding, editing, deleting, and viewing expenses with pagination.
Frontend uses React state and hooks to manage expenses and update the UI in real time.
Spending Insights Endpoint
The backend calculates total spending per category and provides percentage distribution.
Insights are visualized on the frontend using MUI X Charts/Recharts for clear representation of spending patterns.
