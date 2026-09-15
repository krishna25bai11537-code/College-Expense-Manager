# College-Expense-Manager# Smart College Expense Tracker

## 1. Project Overview

Smart College Expense Tracker is a full-stack student financial management application developed as a college project for the **Programming in Java** course.

The project is designed to help college students manage their daily finances in one centralized platform. It provides features for recording expenses, setting budgets, analyzing spending patterns, monitoring financial performance, splitting group expenses, managing recurring expenses, and generating financial reports.

The project combines a modern web interface with a **Java Spring Boot backend** to demonstrate practical application of Java, object-oriented programming, REST APIs, database management, authentication, and full-stack development.

### Main Objective

The main objective of the project is to make personal expense management easier for college students by providing a simple platform where they can:

* Track daily expenses
* Set monthly and category-wise budgets
* Monitor spending patterns
* Receive spending alerts
* Calculate a Student Spending Score
* Split expenses with friends
* Manage recurring payments
* Generate financial reports

---

## 2. Features

### Authentication

* Student registration
* Student login
* JWT-based authentication
* Protected application routes
* User profile management

### Expense Management

* Add expenses
* View expense history
* Search and filter expenses
* Edit expenses
* Delete expenses
* Categorize expenses
* Track payment methods
* Record expense descriptions and dates

### Dashboard

* Monthly spending summary
* Recent transactions
* Budget information
* Spending trends
* Financial alerts
* Student Spending Score

### Budget Management

* Set monthly budget
* Set category-wise budgets
* Track budget utilization
* Monitor remaining budget
* Identify categories approaching their limits

### Analytics

* Category-wise spending analysis
* Weekly spending analysis
* Monthly spending trends
* Historical financial data
* Visual charts and summaries

### Student Spending Score

The application provides a transparent **0–100 Student Spending Score** based on factors such as:

* Budget utilization
* Discretionary spending
* Category budget discipline
* Remaining savings/budget buffer

The score provides students with an easy way to understand their overall spending behavior.

### Smart Spending Alerts

The application can provide alerts related to:

* High spending
* Budget utilization
* Spending spikes
* Low remaining financial buffer

### Expense Splitter

The Expense Splitter helps students manage group expenses such as:

* Group meals
* Trips
* Hostel expenses
* Shared purchases

It calculates participant amounts and helps determine who has paid, who owes money, and the resulting balance.

### Recurring Expenses

Students can maintain recurring expenses such as:

* Subscriptions
* Memberships
* Regular payments
* Monthly expenses

### Reports

* Monthly financial reports
* Category-wise budget comparison
* Financial summaries
* Transaction reports
* CSV export functionality

### User Interface

* Responsive web interface
* Modern fintech-inspired design
* Dark interface
* Dashboard cards
* Interactive charts
* Navigation sidebar
* Modals and notifications
* Responsive layouts

---

## 3. Technologies / Tools Used

### Java

Java is used as the primary backend programming language.

It is used for:

* Object-oriented programming
* Hospital/student-related data modeling
* Business logic
* REST API development
* Exception handling
* Collections
* Authentication
* Database interaction

### Spring Boot

Spring Boot is used to develop the backend REST API and organize the application into controllers, services, repositories, security, DTOs, and entities.

### Spring Security

Spring Security is used for:

* Authentication
* Authorization
* Protected API endpoints
* JWT-based security
* Password protection

### JWT

JSON Web Tokens are used to maintain authenticated sessions between the frontend and backend.

### Spring Data JPA / Hibernate

Used for:

* Database interaction
* Object-relational mapping
* Entity management
* Repository operations

### MySQL

MySQL is used as the primary relational database for storing:

* Users
* Expenses
* Budgets
* Category budgets
* Shared expenses
* Expense participants
* Recurring expenses

### React

React is used to build the frontend interface and create reusable UI components.

### TypeScript

TypeScript is used for structured and type-safe frontend development.

### HTML

HTML is used as part of the frontend structure and component rendering.

### CSS / Tailwind CSS

Used for:

* Styling
* Responsive layouts
* UI components
* Animations
* Modern dashboard design

### JavaScript

JavaScript/TypeScript functionality is used for:

* Frontend interactions
* Navigation
* API communication
* Dynamic content
* Application state

### Vite

Vite is used as the frontend development and build tool.

### Axios

Axios is used for communication between the frontend and backend REST APIs.

### Recharts

Recharts is used to create financial charts and data visualizations.

### OpenCSV

OpenCSV is used to generate CSV reports and export financial information.

### GitHub

GitHub is used for:

* Source-code management
* Version control
* Project submission
* Repository hosting

### Google AI Studio

Google AI Studio was used during the development and design process of the project.

---

# 4. Project Structure

The project is divided into frontend and backend modules.

```text
Smart College Expense Tracker
│
├── frontend
│   ├── src
│   │   ├── components
│   │   ├── context
│   │   ├── pages
│   │   ├── services
│   │   └── types
│   │
│   ├── App.tsx
│   ├── main.tsx
│   └── package.json
│
└── backend
    ├── src
    │   └── main
    │       ├── java
    │       │   └── com
    │       │       └── college
    │       │           └── expensetracker
    │       │               ├── entity
    │       │               ├── repository
    │       │               ├── dto
    │       │               ├── security
    │       │               ├── config
    │       │               ├── exception
    │       │               ├── service
    │       │               └── controller
    │       │
    │       └── resources
    │           ├── application.properties
    │           ├── schema.sql
    │           └── data.sql
    │
    ├── pom.xml
    └── README.md
```

---

# 5. Steps to Install and Run the Project

## Step 1: Clone the Repository

Clone the GitHub repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Replace:

```text
YOUR_GITHUB_REPOSITORY_URL
```

with the actual GitHub repository URL.

---

## Step 2: Open the Project

Open the downloaded project folder using a suitable code editor such as:

* Visual Studio Code
* IntelliJ IDEA
* Eclipse

---

# 6. Backend Setup

## Requirements

Make sure the following are installed:

* Java JDK 17 or above
* Apache Maven 3.8+
* MySQL 8.0+

---

## Step 3: Configure MySQL

Create the project database in MySQL:

```sql
CREATE DATABASE college_expense_db;
```

Update the database configuration in:

```text
backend/src/main/resources/application.properties
```

Enter your MySQL username and password as required by the project configuration.

---

## Step 4: Run the Java Spring Boot Backend

Navigate to the backend folder:

```bash
cd backend
```

Build the project:

```bash
mvn clean install
```

Run the application:

```bash
mvn spring-boot:run
```

The backend runs on:

```text
http://localhost:8080
```

---

# 7. Frontend Setup

## Step 5: Install Node Dependencies

Navigate to the frontend directory:

```bash
cd frontend
```

Install the required packages:

```bash
npm install
```

---

## Step 6: Start the Frontend

Run:

```bash
npm run dev
```

The frontend development server runs on the configured development port.

Open the displayed local URL in your browser.

---

# 8. Testing Instructions

## Web Application Testing

Open the application and test the following modules:

### Authentication

* Registration
* Login
* Logout
* Protected routes
* User profile

### Dashboard

* Monthly summary
* Recent expenses
* Budget information
* Spending score
* Alerts
* Charts

### Expense Management

Test:

* Add expense
* View expenses
* Search expenses
* Filter expenses
* Edit expense
* Delete expense

### Budget Management

Test:

* Monthly budget
* Category budget
* Budget utilization
* Remaining budget

### Analytics

Check:

* Category-wise spending
* Weekly spending
* Monthly spending
* Historical trends
* Charts

### Spending Score

Verify that the application generates a score between:

```text
0 – 100
```

Check the displayed score and its corresponding financial-discipline category.

### Expense Splitter

Test:

* Creating a shared expense
* Adding participants
* Calculating individual shares
* Recording paid amounts
* Checking outstanding balances

### Recurring Expenses

Test:

* Adding recurring expenses
* Weekly/monthly frequency
* Start and end dates
* Removing recurring expenses

### Reports

Test:

* Monthly report
* Category analysis
* Financial summary
* CSV export

---

# 9. Backend Testing

The backend REST APIs should be tested using the application interface or an API testing tool.

Important API areas include:

```text
/api/auth
/api/expenses
/api/dashboard
/api/budget
/api/analytics
/api/spending-score
/api/alerts
/api/shared-expenses
/api/recurring-expenses
/api/reports
```

Verify that:

* Valid requests return successful responses.
* Invalid data is rejected appropriately.
* Protected endpoints require authentication.
* Expense records are stored correctly.
* Budget calculations are correct.
* Reports contain the expected information.

---

# 10. Database Testing

Verify that the following database tables are created correctly:

```text
users
expenses
budgets
category_budgets
shared_expenses
shared_expense_participants
recurring_expenses
```

Check:

* User records
* Expense records
* Budget records
* Category budgets
* Shared expenses
* Participants
* Recurring expenses
* Foreign-key relationships

---

# 11. Java Concepts Demonstrated

The project demonstrates several important Java concepts:

* Classes and Objects
* Encapsulation
* Constructors
* Methods
* Variables and Data Types
* Collections
* Exception Handling
* Custom Exceptions
* Packages
* REST API development
* Spring Boot
* Spring Security
* JWT Authentication
* JPA / Hibernate
* Database Connectivity
* DTOs
* Layered Architecture

The project applies these concepts to a practical financial-management application rather than treating them as isolated programming examples.

---

# 12. Architecture

The basic architecture of the application is:

```text
             STUDENT
                |
                v
       React / TypeScript
          Frontend
                |
          REST API + JWT
                |
                v
        Spring Security
                |
                v
       REST Controllers
                |
                v
        Service Layer
                |
                v
      Repository Layer
                |
                v
       JPA / Hibernate
                |
                v
          MySQL Database
```

This architecture separates the user interface, security, API handling, business logic, and database operations.

---

# 13. Project Highlights

The major highlights of the project are:

* Student-focused financial management
* Full-stack Java application
* Secure JWT authentication
* Persistent MySQL database
* REST API architecture
* Budget tracking
* Financial analytics
* Student Spending Score
* Smart spending alerts
* Group expense splitting
* Recurring expense management
* Monthly financial reports
* CSV export
* Responsive modern interface

---

# 14. Future Enhancements

The project can be further improved by adding:

* Mobile application
* Push notifications
* Email notifications
* Receipt scanning using OCR
* Automatic expense categorization
* UPI/bank statement import
* Advanced financial predictions
* AI-based spending recommendations
* Cloud deployment
* Role-based access
* Advanced authentication
* Automated recurring transaction generation
* More detailed financial dashboards

---

# 15. Conclusion

Smart College Expense Tracker is a full-stack financial management system designed to address the everyday financial challenges faced by college students.

The project combines a modern React and TypeScript frontend with a Java Spring Boot backend, JWT authentication, Spring Data JPA/Hibernate, and MySQL database management.

By integrating expense tracking, budgeting, analytics, spending alerts, a Student Spending Score, expense splitting, recurring expenses, and financial reporting, the application provides a centralized platform for managing student finances.

The project also demonstrates practical implementation of Java and software-development concepts such as object-oriented programming, exception handling, REST APIs, authentication, database connectivity, layered architecture, and modular development.

Overall, the project provides a strong foundation for developing a more advanced personal-finance platform for students in the future.
